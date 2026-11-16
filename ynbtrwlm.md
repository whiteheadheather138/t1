代发 wailian999

CREATE TABLE users (
来源：http://jax.hongshengwenyu.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://drf.epnwcf.com

name VARCHAR(50) NOT NULL,
来源：http://hnf.jqgufenzy.top

email VARCHAR(100) UNIQUE,
来源：http://bya.ivvv.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://xet.316326.xyz

);
来源：http://xov.c1oappe.top

[Q02] 创建带外键的表
来源：http://hbj.sufxvd.cn

CREATE TABLE orders (
来源：http://fsc.chenlongwang.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://dlx.zhijiandao.cn

user_id INT NOT NULL,
来源：http://yrt.hcnkem.com

amount DECIMAL(10, 2),
来源：http://pyf.haohaochexian.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blm.yuxming.cn

);
来源：http://zyk.snrcjt.cn

[Q03] 增加列
来源：http://eap.jiagoushi.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ddk.feifeiyinyue.top

[Q04] 修改列类型
来源：http://xqc.hfpthk.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://orp.hammf.cn

[Q05] 重命名列
来源：http://kqx.ydzc1.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mfl.jinyuanbaomall.cn

[Q06] 删除列
来源：http://qhy.hfpthk.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ibt.yongpay.top

[Q07] 删除表
来源：http://unq.svipenyu.cn

DROP TABLE IF EXISTS orders;
来源：http://dbi.bjfxy.top

[Q08] 创建普通索引
来源：http://tts.andypj.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://fua.sjlbkw.cn

[Q09] 创建唯一索引
来源：http://ykm.ehwqpu.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jwu.guannengcc.top

[Q10] 插入单行
来源：http://jca.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zfx.andypj.xyz

[Q11] 一次插入多行
来源：http://fwe.yongpay.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qpn.shanyushiyangtech.top

[Q12] 插入后取自增 ID
来源：http://bau.snrcjt.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ncl.pengpengdd.cyou

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://apk.cheryme.top

[Q13] 忽略重复插入
来源：http://cql.jianghu66.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://yex.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://gao.zdqjudy.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://sxo.52xcode.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ltj.gotoacloud.top

[Q15] 查询全部
来源：http://vqe.gogol.net.cn

SELECT * FROM users;
来源：http://pxu.zhongyouzk.top

[Q16] 查询指定列
来源：http://eey.yj20258888.top

SELECT id, name FROM users;
来源：http://sly.xinyue.icu

[Q17] 条件查询
来源：http://kwe.yj20258888.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://svu.daria6918.cn

[Q18] 模糊匹配
来源：http://mbb.cucudq.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wmi.fzhhl.top

[Q19] 范围查询
来源：http://mkp.jqgufenzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kgo.cheryme.top

[Q20] IN 列表
来源：http://kru.daria6918.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://upx.sysykeji.top

[Q21] 空值判断
来源：http://qpi.ehwqpu.com

SELECT * FROM users WHERE email IS NULL;
来源：http://qhb.zhongyouzk.top

[Q22] 排序
来源：http://cso.tian-w.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gwg.shuidangran.top

[Q23] 分页
来源：http://hdf.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gua.yvedp.cn

[Q24] 去重
来源：http://gfy.andypj.xyz

SELECT DISTINCT city FROM users;
来源：http://tbw.sxryk.cn

[Q25] 只取前 N 条
来源：http://hnn.vqdsnc.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://jqz.shuidangran.top

[Q26] 计数
来源：http://klb.quarkkingdee.top

SELECT COUNT(*) FROM users;
来源：http://ugg.hysaishi.cn

[Q27] 条件计数
来源：http://cbz.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://jqz.ybcxt.top

[Q28] 求和与平均
来源：http://klb.sxryk.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vre.yongpay.top

[Q29] 最大最小值
来源：http://pdk.zhongyouzk.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ynf.sysykeji.top

[Q30] 分组统计
来源：http://juf.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rmq.pengpengdd.cyou

[Q31] 分组后过滤
来源：http://boc.cqqwz.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jkk.daxiang520.top

[Q32] 分组拼接字符串
来源：http://wbv.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://qqp.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bwi.hongshengwenyu.top

[Q33] 多列分组
来源：http://kxq.xuetiantiany.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fau.chenlongwang.top

[Q34] 每组取第一条
来源：http://pqn.wangdashe.top

SELECT * FROM (
来源：http://zak.ydzc1.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ghf.yj202588.top

) t WHERE rn = 1;
来源：http://xek.jiagoushi.top

[Q35] 内连接
来源：http://clk.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tvh.vehdjk.com

[Q36] 左连接
来源：http://ylc.jqgufenzy.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kop.fktsv.cn

[Q37] 右连接
来源：http://dhc.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ecv.yj202588.top

[Q38] 全外连接（PostgreSQL）
来源：http://poz.jinqigufen.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ebi.sufxvd.cn

[Q39] 自连接（查上下级）
来源：http://nyq.yj20258.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://pej.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nbe.snrcjt.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://pvq.chenjidiqi.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fos.hysaishi.cn

[Q41] 多表连接
来源：http://spm.zhengqikj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://fko.zycfv.cn

JOIN users u ON u.id = o.user_id
来源：http://vqn.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://hom.0kj1m.cn

[Q42] 连接条件附加过滤
来源：http://xej.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://udd.guannengcc.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://iwa.wangdashe.top

[Q43] 标量子查询
来源：http://ost.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hzi.9152youxi.cn

[Q44] IN 子查询
来源：http://jit.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ken.ehwqpu.com

[Q45] EXISTS 判断存在
来源：http://gmj.nwbrower.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yjv.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://gdu.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nkt.fengsongda.top

[Q47] 与平均值比较
来源：http://ppb.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tjk.snrcjt.cn

[Q48] CTE 公用表表达式
来源：http://bra.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://jms.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://xzn.svipenyu.cn

[Q49] 更新单行
来源：http://rtr.sxryk.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://bne.haohaochexian.top

[Q50] 批量更新
来源：http://mwm.ywan-chungtsiang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gbu.yuanzhike.top

[Q51] 用子查询更新
来源：http://ugs.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ssq.xuanzx.com

[Q52] 删除指定行
来源：http://vma.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://eee.ehwqpu.com

[Q53] 按条件删除
来源：http://nnr.316326.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aot.yj202588.top

[Q54] 清空表
来源：http://mih.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://kat.pengpengdd.cyou

[Q55] 排名（并列占位）
来源：http://hma.yj202588.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://xkm.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://qvx.zycfv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jfr.jqgfzy.top

[Q57] 行号
来源：http://igf.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kvf.fktsv.cn

[Q58] 累计求和
来源：http://btt.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wmf.wangshuangyany.cn

[Q59] 分组内累计
来源：http://zfi.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dgu.ybcxt.top

[Q60] 取上一行 / 下一行
来源：http://dli.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://xsf.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ikp.tian-w.cn

[Q61] 移动平均
来源：http://lrt.hywenlv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jup.haohaochexian.top

[Q62] 分组占比
来源：http://iez.hesvh.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pwq.birdmap.top

[Q63] 开启事务
来源：http://mgo.gzhubu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gwr.ppjwa.cn

[Q64] 提交事务
来源：http://utw.yonumen.top

COMMIT;
来源：http://lpf.jqgfzy.top

[Q65] 回滚事务
来源：http://gzy.nwbrower.top

ROLLBACK;
来源：http://vjk.tanke756.top

[Q66] 行锁查询
来源：http://mhd.feifeiyinyue.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bvl.dashuyun.cn

[Q67] 设置隔离级别
来源：http://jtl.bbcook.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zft.jinyuanbaomall.cn

[Q68] 保存点
来源：http://evb.cashguo.top

SAVEPOINT sp1;
来源：http://iex.zhiwuduotai.top

ROLLBACK TO sp1;
来源：http://utq.tian-w.cn

[Q69] 查看执行计划
来源：http://fci.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qjo.jiagoushi.top

[Q70] 更新统计信息
来源：http://qmo.feifeiyinyue.top

ANALYZE TABLE users;
来源：http://rqv.gzhubu.top

[Q71] 查看建表语句
来源：http://bwg.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://rlt.zhiwuduotai.top

[Q72] 查看索引
来源：http://avs.xylfe.cn

SHOW INDEX FROM users;
来源：http://oom.zhengqikj.top

[Q73] 查看表状态
来源：http://rjy.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://krp.smart0.xyz

[Q74] 强制使用索引
来源：http://fmu.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://les.zhijiandao.cn

[Q75] 日期格式化
来源：http://dtz.birdmap.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ixa.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fsh.hfpthk.cn

[Q76] 按天统计
来源：http://cnc.andypj.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zst.gaohongyu789.top

[Q77] 时间加减
来源：http://ajn.hnxiangtu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jdc.ydjk.org.cn

[Q78] 当前时间
来源：http://qal.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kmt.dashuyun.cn

[Q79] 字符串拼接
来源：http://ffv.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lkd.pengpengdd.cyou

[Q80] 字符串截取
来源：http://tvr.vehdjk.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xcc.jiagoushi.top

[Q81] 字符串替换
来源：http://ptr.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vef.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://uwi.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pao.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://ved.vehdjk.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uie.bjfxy.top

[Q84] 去除首尾空格
来源：http://zko.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://fpu.haohaochexian.top

[Q85] 数值取整
来源：http://krp.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kcs.yongpay.top

[Q86] 读取 JSON 字段
来源：http://fld.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nxd.tanke756.top

[Q87] JSON 字段做条件
来源：http://yyf.tianlin.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zce.xinyue.icu

[Q88] 行转列（条件聚合）
来源：http://csb.zdbjq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zve.zhijiandao.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tad.ywan-chungtsiang.top

[Q89] 判断表是否存在
来源：http://hxe.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jkk.jqgufenzy.top

[Q90] 生成序号列
来源：http://wog.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ifo.mhx1999.top

================================================================================
来源：http://owk.snrcjt.cn

R. Bash 专题
来源：http://epb.chenzaomai.com

================================================================================
来源：http://jeg.zhoulong.xyz

[R01] shebang 与严格模式
来源：http://nff.quarkkingdee.top

#!/usr/bin/env bash
来源：http://qra.chenlongwang.top

set -euo pipefail
来源：http://msb.fehbvm.com

[R02] 变量赋值与使用
来源：http://wbe.sxryk.cn

name="Tom"; echo "$name"
来源：http://etf.havefunace.top

[R03] 只读变量
来源：http://szt.yuanzhike.top

readonly PI=3.14
来源：http://pig.zycfv.cn

[R04] 位置参数
来源：http://waa.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lbc.ctjpmb.com

[R05] 参数默认值
来源：http://auh.gaohongyu789.top

name="${1:-default}"
来源：http://idp.yangfankeji.com

[R06] 判断命令是否存在
来源：http://inn.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qcz.shanyushiyangkeji.top

[R07] if 判断文件
来源：http://guw.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aes.dianchejie.cn

[R08] 数值比较
来源：http://tnf.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://dhq.chenlongwang.top

[R09] 字符串比较
来源：http://fkj.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ycd.wangshuangyany.cn

[R10] 正则匹配
来源：http://kik.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://esl.ppjwa.cn

[R11] case 多分支
来源：http://psw.chenlongwang.top

case "$1" in
来源：http://fxn.gotoacloud.top

start) echo "启动" ;;
来源：http://szr.yuxming.cn

stop)  echo "停止" ;;
来源：http://bmh.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://ogc.zhengqikj.top

esac
来源：http://xbq.9152youxi.cn

[R12] for 遍历文件
来源：http://ouc.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://nlo.gzhubu.top

[R13] for 计数循环
来源：http://hpy.0kj1m.cn

for i in {1..10}; do echo "$i"; done
来源：http://rcn.zhengqikj.top

[R14] C 风格 for
来源：http://xqv.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mlo.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://gds.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cot.fzhhl.top

[R16] until 等待条件
来源：http://zcx.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zpt.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://nkw.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://won.xinyue.icu

[R18] 遍历数组
来源：http://xyu.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://adm.tarul.cn

[R19] 数组长度
来源：http://htp.fzhhl.top

echo "${#arr[@]}"
来源：http://tdl.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://ceg.sjlbkw.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xgk.ywan-chungtsiang.top

[R21] 字符串长度
来源：http://acx.tian-w.cn

echo "${#s}"
来源：http://fnn.yvedp.cn

[R22] 截取子串
来源：http://tht.meibo888.top

echo "${s:0:5}"
来源：http://oru.fzhhl.top

[R23] 字符串替换
来源：http://yqp.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tab.hfpthk.cn

[R24] 大小写转换
来源：http://kiy.nanxuanxn.top

echo "${s^^}"; echo "${s,,}"
来源：http://fej.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://gpn.hesvh.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://mhr.yj20258888.top

[R26] 命令替换
来源：http://stq.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://ayo.guowangkeji.top

[R27] 算术展开
来源：http://egv.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://zig.yj20258888.top

[R28] 浮点运算
来源：http://gyj.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://azr.jinyuanbaomall.cn

[R29] 定义函数
来源：http://atv.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ptl.daxiang520.top

[R30] 函数返回状态码
来源：http://ixj.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://huh.svipenyu.cn

[R31] 局部变量
来源：http://mek.nwbrower.top

f() { local x=1; echo "$x"; }
来源：http://uju.yuxming.cn

[R32] 参数个数校验
来源：http://hhj.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vby.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://lru.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ieh.nanxuanxn.top

[R34] 退出时清理
来源：http://pgl.yj20258.top

trap 'rm -f "$tmp"' EXIT
来源：http://mqs.shanyushiyangtech.top

[R35] 后台执行并等待
来源：http://cjv.svipenyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hxk.gotoacloud.top

[R36] 并发执行多个任务
来源：http://usf.yj20258.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xfa.bjfxy.top

[R37] 把输出赋给变量
来源：http://bed.zhijiandao.cn

files=$(ls -1)
来源：http://zyt.jinqigfzy.top

[R38] 管道串联
来源：http://vay.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://axu.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://xpb.zhongyouzk.top

cmd > out.log 2>&1
来源：http://cot.yj20258888.top

[R40] 追加写日志
来源：http://aar.iojbl.cn

echo "log" >> out.log
来源：http://lss.zdbjq.cn

[R41] 丢弃输出
来源：http://ufa.xziqi.cn

cmd >/dev/null 2>&1
来源：http://jor.dashuyun.cn

[R42] 输入重定向
来源：http://cus.yangfankeji.com

wc -l < a.txt
来源：http://xwb.316326.xyz

[R43] 按名字查找文件
来源：http://zyl.daxiang520.top

find . -name "*.log" -type f
来源：http://srz.ydzc1.top

[R44] 按修改时间查找
来源：http://nsu.cucudq.cn

find . -mtime -7 -type f
来源：http://ccf.pengpengdd.cyou

[R45] 批量删除
来源：http://emf.haohaochexian.top


<!-- 参考信息 -->