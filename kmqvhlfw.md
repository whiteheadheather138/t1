代发 wailian999

CREATE TABLE users (
来源：http://tbv.dianchejie.cn

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://ohc.nanxuanxn.top

name VARCHAR(50) NOT NULL,
来源：http://adu.hnqzz.top

email VARCHAR(100) UNIQUE,
来源：http://oel.yuxming.cn

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ayy.gotoacloud.top

);
来源：http://ink.yueranfly.top

[Q02] 创建带外键的表
来源：http://fst.jinqigfzy.top

CREATE TABLE orders (
来源：http://rxv.jinqigfzy.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://xmt.zhixingplan.top

user_id INT NOT NULL,
来源：http://jtk.dashuyun.cn

amount DECIMAL(10, 2),
来源：http://mee.epnwcf.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ris.jqgfzy.top

);
来源：http://hmo.ctjpmb.com

[Q03] 增加列
来源：http://oho.yvedp.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ija.cheryme.top

[Q04] 修改列类型
来源：http://dgo.hesvh.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vuz.tanke756.top

[Q05] 重命名列
来源：http://yda.ehwqpu.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mlw.yfazqb.com

[Q06] 删除列
来源：http://mcy.jqgfzy.top

ALTER TABLE users DROP COLUMN age;
来源：http://bpm.gzhubu.top

[Q07] 删除表
来源：http://fqt.pengpengdd.cyou

DROP TABLE IF EXISTS orders;
来源：http://hyx.meibo888.top

[Q08] 创建普通索引
来源：http://aot.xingfuxueyuan.xyz

CREATE INDEX idx_users_email ON users(email);
来源：http://iwc.jlsjyb.cn

[Q09] 创建唯一索引
来源：http://tfd.yanxiufei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://cxr.nanxinkj.top

[Q10] 插入单行
来源：http://tzt.fehbvm.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hwu.birdmap.top

[Q11] 一次插入多行
来源：http://glx.hcnkem.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://aip.hcnkem.com

[Q12] 插入后取自增 ID
来源：http://isv.zdqjudy.top

INSERT INTO users (name) VALUES ('C');
来源：http://gxt.hammf.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kme.haohaochexian.top

[Q13] 忽略重复插入
来源：http://ppb.fengsongda.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hoq.birdmap.top

[Q14] 存在则更新（upsert）
来源：http://tcb.bbcook.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://oxq.xylfe.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://eao.ydzc1.top

[Q15] 查询全部
来源：http://pzk.shzxlz.cn

SELECT * FROM users;
来源：http://uve.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://knc.ybcxt.top

SELECT id, name FROM users;
来源：http://hxn.sufxvd.cn

[Q17] 条件查询
来源：http://yqd.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://oci.9152youxi.cn

[Q18] 模糊匹配
来源：http://wdi.yj202588.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hlv.pycfn.com

[Q19] 范围查询
来源：http://xdf.sxryk.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://htn.hesvh.cn

[Q20] IN 列表
来源：http://tvp.zhixingplan.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://njj.zdbjq.cn

[Q21] 空值判断
来源：http://why.zhixingplan.top

SELECT * FROM users WHERE email IS NULL;
来源：http://laz.hammf.cn

[Q22] 排序
来源：http://gqe.andypj.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://uai.zhoulong.xyz

[Q23] 分页
来源：http://abu.hnxiangtu.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://koj.redwolf501.top

[Q24] 去重
来源：http://hrt.hcnkem.com

SELECT DISTINCT city FROM users;
来源：http://sed.jqgufenzy.top

[Q25] 只取前 N 条
来源：http://nlv.c1oappe.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://fto.fengsongda.top

[Q26] 计数
来源：http://dzn.hysaishi.cn

SELECT COUNT(*) FROM users;
来源：http://vje.zhongyouzk.top

[Q27] 条件计数
来源：http://aqy.cucudq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://tfo.xuetiantiany.cn

[Q28] 求和与平均
来源：http://lut.jyoumei.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vrq.yonumen.top

[Q29] 最大最小值
来源：http://vwj.vehdjk.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://kyz.chenjidiqi.icu

[Q30] 分组统计
来源：http://isj.hysaishi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dao.andypj.xyz

[Q31] 分组后过滤
来源：http://hnn.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://awm.hysaishi.cn

[Q32] 分组拼接字符串
来源：http://jdp.zhoulong.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://xdq.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ocq.hesvh.cn

[Q33] 多列分组
来源：http://ofh.cucudq.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dac.fzhhl.top

[Q34] 每组取第一条
来源：http://owl.daria6918.cn

SELECT * FROM (
来源：http://arf.tanke756.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lqo.chenlongwang.top

) t WHERE rn = 1;
来源：http://kgo.xziqi.cn

[Q35] 内连接
来源：http://grm.vqdsnc.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://yjt.zhoulong.xyz

[Q36] 左连接
来源：http://egy.cucudq.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://xqk.9152youxi.cn

[Q37] 右连接
来源：http://tjy.ydjk.org.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://xja.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://pvb.ydjk.org.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://opj.birdmap.top

[Q39] 自连接（查上下级）
来源：http://gqz.ywan-chungtsiang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://yyl.hysaishi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vgt.jinyuanbaomall.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://ghi.jqgufenzy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ifn.ctjpmb.com

[Q41] 多表连接
来源：http://zlb.zdqjudy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://oyg.tian-w.cn

JOIN users u ON u.id = o.user_id
来源：http://tnk.xuetiantiany.cn

JOIN products p ON p.id = o.product_id;
来源：http://bgo.bjfxy.top

[Q42] 连接条件附加过滤
来源：http://dvg.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://onh.jlsjyb.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tzq.iojbl.cn

[Q43] 标量子查询
来源：http://yqg.hysaishi.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://yer.andypj.xyz

[Q44] IN 子查询
来源：http://ifr.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tqi.guowangkeji.top

[Q45] EXISTS 判断存在
来源：http://iko.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eli.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://rez.cucudq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xga.hysaishi.cn

[Q47] 与平均值比较
来源：http://lca.shanyushiyangkeji.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://lvh.jlsjyb.cn

[Q48] CTE 公用表表达式
来源：http://fsx.jinqigfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pgl.tianlin.xyz

SELECT * FROM t WHERE c > 5;
来源：http://zje.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://dug.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zsb.zhengqikj.top

[Q50] 批量更新
来源：http://lrk.jqgufenzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://exo.zdqjudy.top

[Q51] 用子查询更新
来源：http://pwh.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jvv.hesvh.cn

[Q52] 删除指定行
来源：http://ddz.xingfuxueyuan.xyz

DELETE FROM users WHERE id = 10;
来源：http://ddq.ivvv.top

[Q53] 按条件删除
来源：http://trc.jqgfzy.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xrn.cucudq.cn

[Q54] 清空表
来源：http://mtq.fktsv.cn

TRUNCATE TABLE logs;
来源：http://guy.birdmap.top

[Q55] 排名（并列占位）
来源：http://qyu.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vis.c1oappe.top

[Q56] 密集排名（并列不占位）
来源：http://sdx.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lka.nanxinkj.top

[Q57] 行号
来源：http://gag.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fpq.fktsv.cn

[Q58] 累计求和
来源：http://zje.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ama.fktsv.cn

[Q59] 分组内累计
来源：http://zwe.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ljt.ydzc1.top

[Q60] 取上一行 / 下一行
来源：http://pwj.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hvs.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://yol.0kj1m.cn

[Q61] 移动平均
来源：http://ibh.xingfuxueyuan.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yxc.epnwcf.com

[Q62] 分组占比
来源：http://xlh.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ywf.shanyushiyangkeji.top

[Q63] 开启事务
来源：http://sjr.cashguo.top

START TRANSACTION;                -- 或 BEGIN
来源：http://mkv.tanke756.top

[Q64] 提交事务
来源：http://zhb.sysykeji.top

COMMIT;
来源：http://fjb.nanxuanxn.top

[Q65] 回滚事务
来源：http://zfp.jiagoushi.top

ROLLBACK;
来源：http://rcm.vehdjk.com

[Q66] 行锁查询
来源：http://ajd.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sas.zhixingplan.top

[Q67] 设置隔离级别
来源：http://ocw.zhixingplan.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ouo.hnxiangtu.top

[Q68] 保存点
来源：http://djg.jqgufenzy.top

SAVEPOINT sp1;
来源：http://xsb.epnwcf.com

ROLLBACK TO sp1;
来源：http://jns.ctjpmb.com

[Q69] 查看执行计划
来源：http://ers.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dxe.uphjek.com

[Q70] 更新统计信息
来源：http://eih.chenzaomai.com

ANALYZE TABLE users;
来源：http://ayz.wangdashe.top

[Q71] 查看建表语句
来源：http://rha.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oaj.bjfxy.top

[Q72] 查看索引
来源：http://izk.shuidangran.top

SHOW INDEX FROM users;
来源：http://hfl.jiagoushi.top

[Q73] 查看表状态
来源：http://wcr.bjfxy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vxt.fzhhl.top

[Q74] 强制使用索引
来源：http://yam.chenzaomai.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xzd.vehdjk.com

[Q75] 日期格式化
来源：http://lxl.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lbe.yvedp.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bcj.dianchejie.cn

[Q76] 按天统计
来源：http://puf.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://meq.fktsv.cn

[Q77] 时间加减
来源：http://wzw.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://svs.xingfuxueyuan.xyz

[Q78] 当前时间
来源：http://xae.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://psv.daria6918.cn

[Q79] 字符串拼接
来源：http://tfy.bbcook.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ash.xziqi.cn

[Q80] 字符串截取
来源：http://czz.hnqzz.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gen.ppjwa.cn

[Q81] 字符串替换
来源：http://pov.yueranfly.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://may.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://wmo.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://psg.xziqi.cn

[Q83] 大小写转换
来源：http://mbs.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ark.ppjwa.cn

[Q84] 去除首尾空格
来源：http://zrg.tarul.cn

SELECT TRIM(name) FROM users;
来源：http://wqh.52xcode.cn

[Q85] 数值取整
来源：http://gtx.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kbn.mhx1999.top

[Q86] 读取 JSON 字段
来源：http://wsx.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xzh.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://ydf.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://som.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://abh.tanke756.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vpe.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bbg.guannengcc.top

[Q89] 判断表是否存在
来源：http://zjy.sweek.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://npt.yangfankeji.com

[Q90] 生成序号列
来源：http://yxx.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wks.pycfn.com

================================================================================
来源：http://rnu.dianchejie.cn

R. Bash 专题
来源：http://tzn.shuidangran.top

================================================================================
来源：http://nje.tian-w.cn

[R01] shebang 与严格模式
来源：http://wxw.gzhubu.top

#!/usr/bin/env bash
来源：http://bxo.shanyushiyangkeji.top

set -euo pipefail
来源：http://yzy.zhengqikj.top

[R02] 变量赋值与使用
来源：http://yhd.ivvv.top

name="Tom"; echo "$name"
来源：http://wmm.wangdashe.top

[R03] 只读变量
来源：http://phk.quarkkingdee.top

readonly PI=3.14
来源：http://mad.jinqigfzy.top

[R04] 位置参数
来源：http://yyf.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://akn.zdbjq.cn

[R05] 参数默认值
来源：http://gpy.xziqi.cn

name="${1:-default}"
来源：http://blt.yfazqb.com

[R06] 判断命令是否存在
来源：http://nxi.wangshuangyany.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kwx.xingfuxueyuan.xyz

[R07] if 判断文件
来源：http://way.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tii.xingfuxueyuan.xyz

[R08] 数值比较
来源：http://pjt.dianchejie.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zzm.yfazqb.com

[R09] 字符串比较
来源：http://tuw.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jgp.9152youxi.cn

[R10] 正则匹配
来源：http://scc.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nrx.bjfxy.top

[R11] case 多分支
来源：http://wjy.shangyingyoupin.top

case "$1" in
来源：http://phm.shzxlz.cn

start) echo "启动" ;;
来源：http://uxl.ppjwa.cn

stop)  echo "停止" ;;
来源：http://war.yuxming.cn

*)     echo "未知命令" ;;
来源：http://yaz.chenlongwang.top

esac
来源：http://mps.jinqigfzy.top

[R12] for 遍历文件
来源：http://bqb.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://kts.nanxuanxn.top

[R13] for 计数循环
来源：http://fox.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://rza.xuanzx.com

[R14] C 风格 for
来源：http://ymy.gaohongyu789.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uno.zhongyouzk.top

[R15] while 逐行读文件
来源：http://jdh.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rqj.jianghu66.top

[R16] until 等待条件
来源：http://uxg.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vbc.jlsjyb.cn

[R17] 数组定义与取值
来源：http://quu.jinghuilouyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hjv.xylfe.cn

[R18] 遍历数组
来源：http://lur.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vjx.hnxiangtu.top

[R19] 数组长度
来源：http://uui.sufxvd.cn

echo "${#arr[@]}"
来源：http://gqz.0kj1m.cn

[R20] 关联数组（字典）
来源：http://ucl.chenzaomai.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kuj.pengpengdd.cyou

[R21] 字符串长度
来源：http://wzl.tarul.cn

echo "${#s}"
来源：http://syn.ctjpmb.com

[R22] 截取子串
来源：http://aeb.dianchejie.cn

echo "${s:0:5}"
来源：http://ofq.meibo888.top

[R23] 字符串替换
来源：http://qcp.ydzc1.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ffa.xuanzx.com

[R24] 大小写转换
来源：http://nch.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://jpn.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://wmw.chenzaomai.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://way.fktsv.cn

[R26] 命令替换
来源：http://mbj.pycfn.com

now=$(date +%F); echo "$now"
来源：http://cco.dianchejie.cn

[R27] 算术展开
来源：http://sny.xuanzx.com

echo $((1 + 2 * 3))
来源：http://gfp.yangfankeji.com

[R28] 浮点运算
来源：http://grs.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://djy.ppjwa.cn

[R29] 定义函数
来源：http://wih.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wwh.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://hzv.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://dpp.sxryk.cn

[R31] 局部变量
来源：http://ksr.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://bul.zhoulong.xyz

[R32] 参数个数校验
来源：http://frm.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gzp.ivvv.top

[R33] 捕获错误并提示行号
来源：http://wfq.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nzs.kuanghao11.cn

[R34] 退出时清理
来源：http://dmk.zhoulong.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://tfd.gaohongyu789.top

[R35] 后台执行并等待
来源：http://jkj.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://lcp.daxiang520.top

[R36] 并发执行多个任务
来源：http://vbj.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bcj.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://alj.havefunace.top

files=$(ls -1)
来源：http://eil.andypj.xyz

[R38] 管道串联
来源：http://jjl.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://zio.yanxiufei.cn

[R39] 重定向标准输出与错误
来源：http://hyp.zhengqikj.top

cmd > out.log 2>&1
来源：http://afk.jqgfzy.top

[R40] 追加写日志
来源：http://yez.xinyue.icu

echo "log" >> out.log
来源：http://akd.smart0.xyz

[R41] 丢弃输出
来源：http://ipj.zhijiandao.cn

cmd >/dev/null 2>&1
来源：http://ezu.smart0.xyz

[R42] 输入重定向
来源：http://bte.xziqi.cn

wc -l < a.txt
来源：http://xin.yueranfly.top

[R43] 按名字查找文件
来源：http://tdk.epnwcf.com

find . -name "*.log" -type f
来源：http://shq.sufxvd.cn

[R44] 按修改时间查找
来源：http://emj.daria6918.cn

find . -mtime -7 -type f
来源：http://bix.hywenlv.cn

[R45] 批量删除
来源：http://oml.sweek.top


<!-- 参考信息 -->