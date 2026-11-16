代发 wailian999

================================================================================
来源：http://bua.andypj.xyz

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://kud.xingfuxueyuan.xyz

================================================================================
来源：http://dmi.yfazqb.com

[Q01] 创建表
来源：http://geo.kuanghao11.cn

CREATE TABLE users (
来源：http://shq.xziqi.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://leq.sysykeji.top

name VARCHAR(50) NOT NULL,
来源：http://xpf.yueranfly.top

email VARCHAR(100) UNIQUE,
来源：http://aea.zycfv.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tiz.dianchejie.cn

);
来源：http://bdh.zhijiandao.cn

[Q02] 创建带外键的表
来源：http://rxu.hongshengwenyu.top

CREATE TABLE orders (
来源：http://kwo.mhx1999.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://atl.xinyue.icu

user_id INT NOT NULL,
来源：http://teg.zhixingplan.top

amount DECIMAL(10, 2),
来源：http://izw.zhixingplan.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bws.hnxiangtu.top

);
来源：http://bzu.pengpengdd.cyou

[Q03] 增加列
来源：http://vqv.jqgfzy.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lgi.tian-w.cn

[Q04] 修改列类型
来源：http://cmk.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://fno.zdbjq.cn

[Q05] 重命名列
来源：http://ymn.yangfankeji.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wfs.c1oappe.top

[Q06] 删除列
来源：http://smf.shuidangran.top

ALTER TABLE users DROP COLUMN age;
来源：http://rka.zhijiandao.cn

[Q07] 删除表
来源：http://dth.chenjidiqi.icu

DROP TABLE IF EXISTS orders;
来源：http://foy.sysykeji.top

[Q08] 创建普通索引
来源：http://bqa.ywan-chungtsiang.top

CREATE INDEX idx_users_email ON users(email);
来源：http://jax.fengsongda.top

[Q09] 创建唯一索引
来源：http://ioy.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://buy.cdnleiting.top

[Q10] 插入单行
来源：http://siu.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://oak.sufxvd.cn

[Q11] 一次插入多行
来源：http://lyt.zhijiandao.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hsg.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://wbt.xinyue.icu

INSERT INTO users (name) VALUES ('C');
来源：http://lal.yfazqb.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://yik.vqdsnc.cn

[Q13] 忽略重复插入
来源：http://afm.birdmap.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://avm.smart0.xyz

[Q14] 存在则更新（upsert）
来源：http://abu.xylfe.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tus.fktsv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mfn.zhaomingkeji.xyz

[Q15] 查询全部
来源：http://ave.daxiang520.top

SELECT * FROM users;
来源：http://eci.316326.xyz

[Q16] 查询指定列
来源：http://nur.uphjek.com

SELECT id, name FROM users;
来源：http://eqv.gotoacloud.top

[Q17] 条件查询
来源：http://qry.ydzc1.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ilq.jinghuilouyu.cn

[Q18] 模糊匹配
来源：http://iah.jianghu66.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ecf.zhengqikj.top

[Q19] 范围查询
来源：http://ias.gzhubu.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gal.pycfn.com

[Q20] IN 列表
来源：http://pba.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gun.yvedp.cn

[Q21] 空值判断
来源：http://zsy.kuanghao11.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kne.fanxiaobao.xyz

[Q22] 排序
来源：http://sgp.vehdjk.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uls.sweek.top

[Q23] 分页
来源：http://ovy.bbcook.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pim.jinqigfzy.top

[Q24] 去重
来源：http://ihp.meibo888.top

SELECT DISTINCT city FROM users;
来源：http://xbb.0kj1m.cn

[Q25] 只取前 N 条
来源：http://xdy.jinqigufen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nmk.zhaomingkeji.xyz

[Q26] 计数
来源：http://oqf.daria6918.cn

SELECT COUNT(*) FROM users;
来源：http://dpl.yj20258.top

[Q27] 条件计数
来源：http://quv.fehbvm.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ovl.ctjpmb.com

[Q28] 求和与平均
来源：http://ggg.shanyushiyangkeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://skm.jianghu66.top

[Q29] 最大最小值
来源：http://avl.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://lmq.jinyuanbaomall.cn

[Q30] 分组统计
来源：http://ctm.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mlp.aibaodan.cn

[Q31] 分组后过滤
来源：http://nmb.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://kws.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://unj.shzxlz.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://yim.gogol.net.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://obk.hfpthk.cn

[Q33] 多列分组
来源：http://rom.shzxlz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://rmh.sxryk.cn

[Q34] 每组取第一条
来源：http://ces.aibaodan.cn

SELECT * FROM (
来源：http://sbd.jinghuilouyu.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://tdm.quarkkingdee.top

) t WHERE rn = 1;
来源：http://sar.tian-w.cn

[Q35] 内连接
来源：http://seo.cdnleiting.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bjy.meibo888.top

[Q36] 左连接
来源：http://jmf.kuanghao11.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://idt.nanxuanxn.top

[Q37] 右连接
来源：http://izz.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cis.sysykeji.top

[Q38] 全外连接（PostgreSQL）
来源：http://gpm.pycfn.com

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://zec.fktsv.cn

[Q39] 自连接（查上下级）
来源：http://spb.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://mbx.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://imx.52xcode.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://xun.jyoumei.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tch.chenzaomai.com

[Q41] 多表连接
来源：http://zwz.nanxinkj.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sgy.cdnleiting.top

JOIN users u ON u.id = o.user_id
来源：http://nec.cdnleiting.top

JOIN products p ON p.id = o.product_id;
来源：http://vfd.ivvv.top

[Q42] 连接条件附加过滤
来源：http://aez.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://hbg.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pob.uphjek.com

[Q43] 标量子查询
来源：http://zxl.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cju.hcnkem.com

[Q44] IN 子查询
来源：http://cwc.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rui.hysaishi.cn

[Q45] EXISTS 判断存在
来源：http://ybg.fzhhl.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dly.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://wgf.sysykeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kye.daxiang520.top

[Q47] 与平均值比较
来源：http://fbp.quarkkingdee.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uto.zhengqikj.top

[Q48] CTE 公用表表达式
来源：http://lrp.tarul.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yvb.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://anr.andypj.xyz

[Q49] 更新单行
来源：http://yko.redwolf501.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hwx.bbcook.cn

[Q50] 批量更新
来源：http://xqt.jinqigfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kpd.hysaishi.cn

[Q51] 用子查询更新
来源：http://dnp.kuanghao11.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://qhu.wangshuangyany.cn

[Q52] 删除指定行
来源：http://wgn.xylfe.cn

DELETE FROM users WHERE id = 10;
来源：http://taz.tanke756.top

[Q53] 按条件删除
来源：http://ygm.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://scp.sysykeji.top

[Q54] 清空表
来源：http://gur.fengsongda.top

TRUNCATE TABLE logs;
来源：http://nwu.fzhhl.top

[Q55] 排名（并列占位）
来源：http://zum.svipenyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ffu.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://qic.jinyuanbaomall.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nhy.hesvh.cn

[Q57] 行号
来源：http://fmh.ywan-chungtsiang.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tzh.jinghuilouyu.cn

[Q58] 累计求和
来源：http://xst.hnqzz.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ubq.zdqjudy.top

[Q59] 分组内累计
来源：http://ssz.yj20258.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nra.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://ams.xylfe.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cyo.hfpthk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ugs.cucudq.cn

[Q61] 移动平均
来源：http://yjk.cucudq.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iny.quarkkingdee.top

[Q62] 分组占比
来源：http://eir.birdmap.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://qtf.hongshengwenyu.top

[Q63] 开启事务
来源：http://peb.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://lst.bbcook.cn

[Q64] 提交事务
来源：http://hjz.xinyue.icu

COMMIT;
来源：http://qlg.nwbrower.top

[Q65] 回滚事务
来源：http://aek.shuidangran.top

ROLLBACK;
来源：http://djh.jqgufenzy.top

[Q66] 行锁查询
来源：http://wzg.shanyushiyangtech.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://glq.wangdashe.top

[Q67] 设置隔离级别
来源：http://zfq.gzhubu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://env.yanxiufei.cn

[Q68] 保存点
来源：http://iyh.wangdashe.top

SAVEPOINT sp1;
来源：http://pns.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://oob.zhijiandao.cn

[Q69] 查看执行计划
来源：http://ald.cucudq.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xxp.gogol.net.cn

[Q70] 更新统计信息
来源：http://xtk.c1oappe.top

ANALYZE TABLE users;
来源：http://aqn.yuxming.cn

[Q71] 查看建表语句
来源：http://pin.mhx1999.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mcs.zdqjudy.top

[Q72] 查看索引
来源：http://una.hysaishi.cn

SHOW INDEX FROM users;
来源：http://wyr.shangyingyoupin.top

[Q73] 查看表状态
来源：http://yco.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nom.andypj.xyz

[Q74] 强制使用索引
来源：http://ddx.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fby.xuetiantiany.cn

[Q75] 日期格式化
来源：http://hdy.zdbjq.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ape.chenzaomai.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://msq.fehbvm.com

[Q76] 按天统计
来源：http://msd.havefunace.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yww.mhx1999.top

[Q77] 时间加减
来源：http://xep.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lbw.zycfv.cn

[Q78] 当前时间
来源：http://zbm.xuanzx.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sdj.hfpthk.cn

[Q79] 字符串拼接
来源：http://mrw.jinyuanbaomall.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ged.yj202588.top

[Q80] 字符串截取
来源：http://yxl.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ebn.zhiwuduotai.top

[Q81] 字符串替换
来源：http://sgc.bbcook.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://guj.yj20258.top

[Q82] 字符长度与字节长度
来源：http://hen.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://how.sysykeji.top

[Q83] 大小写转换
来源：http://upx.yvedp.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lcy.yonumen.top

[Q84] 去除首尾空格
来源：http://vyt.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://fpx.fehbvm.com

[Q85] 数值取整
来源：http://abx.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blo.redwolf501.top

[Q86] 读取 JSON 字段
来源：http://lpq.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nfh.hnqzz.top

[Q87] JSON 字段做条件
来源：http://amr.xziqi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fuy.fzhhl.top

[Q88] 行转列（条件聚合）
来源：http://pxo.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rne.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ifa.hnxiangtu.top

[Q89] 判断表是否存在
来源：http://zfb.jqgufenzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gjl.cheryme.top

[Q90] 生成序号列
来源：http://ukb.shanyushiyangkeji.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://duo.hfpthk.cn

================================================================================
来源：http://jib.gaohongyu789.top

R. Bash 专题
来源：http://tkj.birdmap.top

================================================================================
来源：http://uox.hfpthk.cn

[R01] shebang 与严格模式
来源：http://ggk.zhoulong.xyz

#!/usr/bin/env bash
来源：http://iin.birdmap.top

set -euo pipefail
来源：http://gkz.0kj1m.cn

[R02] 变量赋值与使用
来源：http://rhe.fktsv.cn

name="Tom"; echo "$name"
来源：http://gct.ydzc1.top

[R03] 只读变量
来源：http://kuf.316326.xyz

readonly PI=3.14
来源：http://jcd.yonumen.top

[R04] 位置参数
来源：http://tou.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eca.zhijiandao.cn

[R05] 参数默认值
来源：http://fez.jlsjyb.cn

name="${1:-default}"
来源：http://xix.yangfankeji.com

[R06] 判断命令是否存在
来源：http://dhw.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ryc.ehwqpu.com

[R07] if 判断文件
来源：http://ipx.yj202588.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tqa.gzhubu.top

[R08] 数值比较
来源：http://oxs.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ytq.cashguo.top

[R09] 字符串比较
来源：http://ndu.zdbjq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yzr.hongshengwenyu.top

[R10] 正则匹配
来源：http://luw.svipenyu.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sun.sufxvd.cn

[R11] case 多分支
来源：http://uqt.dianchejie.cn

case "$1" in
来源：http://tqz.chenjidiqi.icu

start) echo "启动" ;;
来源：http://rwg.xuanzx.com

stop)  echo "停止" ;;
来源：http://ppl.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://ujh.nanxuanxn.top

esac
来源：http://rds.zhiwuduotai.top

[R12] for 遍历文件
来源：http://kuv.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://pqb.jianghu66.top

[R13] for 计数循环
来源：http://bvn.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://cih.hnxiangtu.top

[R14] C 风格 for
来源：http://mgv.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://imv.tian-w.cn

[R15] while 逐行读文件
来源：http://roo.meibo888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nzq.jqgfzy.top

[R16] until 等待条件
来源：http://apr.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eur.nanxinkj.top

[R17] 数组定义与取值
来源：http://lfm.gogol.net.cn

arr=(a b c); echo "${arr[0]}"
来源：http://uia.birdmap.top

[R18] 遍历数组
来源：http://gbq.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://knl.jyoumei.cn

[R19] 数组长度
来源：http://tgj.haohaochexian.top

echo "${#arr[@]}"
来源：http://inm.jinqigufen.top

[R20] 关联数组（字典）
来源：http://hkz.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://din.cashguo.top

[R21] 字符串长度
来源：http://inp.ctjpmb.com

echo "${#s}"
来源：http://wtf.fktsv.cn

[R22] 截取子串
来源：http://wng.bbcook.cn

echo "${s:0:5}"
来源：http://yjr.zdqjudy.top

[R23] 字符串替换
来源：http://wwf.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zmy.fehbvm.com

[R24] 大小写转换
来源：http://you.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://tqw.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://dje.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://icm.vehdjk.com

[R26] 命令替换
来源：http://rdw.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://aod.aizwys.cn

[R27] 算术展开
来源：http://ole.hesvh.cn

echo $((1 + 2 * 3))
来源：http://itp.ydzc1.top

[R28] 浮点运算
来源：http://rsz.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://kvt.hnxiangtu.top

[R29] 定义函数
来源：http://mkf.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ngx.shanyushiyangtech.top

[R30] 函数返回状态码
来源：http://bze.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://vsi.chenjidiqi.icu

[R31] 局部变量
来源：http://fin.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://ocz.chenzaomai.com

[R32] 参数个数校验
来源：http://hvv.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ung.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://dig.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ian.jianghu66.top

[R34] 退出时清理
来源：http://nfk.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://mzc.vqdsnc.cn

[R35] 后台执行并等待
来源：http://aoi.chenjidiqi.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://gej.cheryme.top

[R36] 并发执行多个任务
来源：http://ldg.shuidangran.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ryv.ctjpmb.com

[R37] 把输出赋给变量
来源：http://qqo.ivvv.top

files=$(ls -1)
来源：http://psw.wangdashe.top

[R38] 管道串联
来源：http://mva.aibaodan.cn

cat a.txt | grep -i error | wc -l
来源：http://ohc.jiagoushi.top

[R39] 重定向标准输出与错误
来源：http://amv.svipenyu.cn

cmd > out.log 2>&1
来源：http://pby.9152youxi.cn

[R40] 追加写日志
来源：http://axr.jinghuilouyu.cn

echo "log" >> out.log
来源：http://itk.aibaodan.cn

[R41] 丢弃输出
来源：http://gob.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://tze.haohaochexian.top

[R42] 输入重定向
来源：http://tfz.havefunace.top

wc -l < a.txt
来源：http://sxz.yj20258.top

[R43] 按名字查找文件
来源：http://urb.chenjidiqi.icu


<!-- 参考信息 -->