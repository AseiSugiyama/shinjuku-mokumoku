# Takumi Kondo

## ��Ђ�Ɩ��ŕ��i����Ă��邱��
PHP, VBA, Java�Ɠ]�X�Ƃ��Ȃ���Ɩ������Ȃ��Ă��܂����B
1������Г��|�[�^���T�C�g���쐬���Ă��܂��B�iJava/Spring�j
�t�����g�G���h�������ł���A�G���G���W�j�A�ł��B

## ���k���邩������Ȃ�����
�E����FJava, PHP, VBA, JavaScript, BootStrap
�EDB�@�FMySQL

## ������邱��
Spring�{�̊w�K�i8�́FSpring JDBC�j

## ���k���邩������Ȃ�����
Java, Spring�ɂ���

## �����̐���

��JdbcTeplate�̊w�K

�EMap�Ŏ擾����
  �P��FMap<String, Object>
�@�����FList<Map<String, Object>>

�E�Ǝ��I�u�W�F�N�g�Ŏ擾����Mapper�iRowMapper�j
  �P��FUser
�@�����FList<User>
�@���Ǝ��I�u�W�F�N�g��RowMapper�̏������K�v

�E�Ǝ��I�u�W�F�N�g�Ŏ擾����Mapper�iBeanPropertyRowMapper�j
  �P��FUser
�@�����FList<User>
�@���Ǝ��I�u�W�F�N�g��RowMapper�̏����͕s�v�����A
�@�@���̃I�u�W�F�N�g��Default Constructor �� Setter���K�v

�i�����j
setter��r�����A���S�R���X�g���N�^��ValueObject�ɂł���
RowMapper���l�I�ɂ͍D���ł��B


��NamedParameterJdbcTemplate�̊w�K
JdbcTeplate�́A?�̌��Ə��ԂŃo�C���h����B
NamedParameterJdbcTemplate�́A�o�C���h���閼�̂��w�肷��B

JdbcTeplate�̏ꍇ
�@String sql = "SELECT * FROM users WHERE id = ? AND param = ?";
�@jdbcTemplate.queryForMap(sql, userId, userParam);
�@
NamedParameterJdbcTemplate�̏ꍇ
�@String sql = "SELECT * FROM users WHERE id = :id AND param = :param";
�@SqlParameterSource paramMap = new MapSqlParameterSource()
  	.addValue("id", userId)
  	.addValue("param", userParam);

�i�����j
�ǂ��ɉ����o�C���h���Ă��邩���킩��Ղ��A
NamedParameterJdbcTemplate�̕����l�I�ɂ͍D���ł��B
