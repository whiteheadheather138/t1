代发 wailian999

CREATE TABLE users (
来源：http://xqw.cdnleiting.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://tet.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://zul.sufxvd.cn

email VARCHAR(100) UNIQUE,
来源：http://ogz.zdqjudy.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vqi.dianchejie.cn

);
来源：http://gfg.sysykeji.top

[Q02] 创建带外键的表
来源：http://yid.chenzaomai.com

CREATE TABLE orders (
来源：http://gtz.cdnleiting.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zzm.shuidangran.top

user_id INT NOT NULL,
来源：http://ypu.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://wuu.fengsongda.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://eyx.svipenyu.cn

);
来源：http://bcy.bbcook.cn

[Q03] 增加列
来源：http://wfg.zhongyouzk.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ghi.cucudq.cn

[Q04] 修改列类型
来源：http://mjh.birdmap.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://pel.ywan-chungtsiang.top

[Q05] 重命名列
来源：http://yel.jqgufenzy.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://eud.havefunace.top

[Q06] 删除列
来源：http://whx.bjfxy.top

ALTER TABLE users DROP COLUMN age;
来源：http://dob.dianchejie.cn

[Q07] 删除表
来源：http://cvg.hesvh.cn

DROP TABLE IF EXISTS orders;
来源：http://jid.haohaochexian.top

[Q08] 创建普通索引
来源：http://drh.yj202588.top

CREATE INDEX idx_users_email ON users(email);
来源：http://dad.andypj.xyz

[Q09] 创建唯一索引
来源：http://rny.zycfv.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://jmh.kuanghao11.cn

[Q10] 插入单行
来源：http://yqw.jinghuilouyu.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://lxo.yfazqb.com

[Q11] 一次插入多行
来源：http://jup.hysaishi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://zda.jqgufenzy.top

[Q12] 插入后取自增 ID
来源：http://vdn.316326.xyz

INSERT INTO users (name) VALUES ('C');
来源：http://ndf.chenjidiqi.icu

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://jmu.jinqigufen.top

[Q13] 忽略重复插入
来源：http://oqu.hysaishi.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ock.gaohongyu789.top

[Q14] 存在则更新（upsert）
来源：http://jkl.gogol.net.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://fkx.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://rwp.52xcode.cn

[Q15] 查询全部
来源：http://irr.fengsongda.top

SELECT * FROM users;
来源：http://jyv.uphjek.com

[Q16] 查询指定列
来源：http://ynf.andypj.xyz

SELECT id, name FROM users;
来源：http://grh.nanxinkj.top

[Q17] 条件查询
来源：http://mnj.sjlbkw.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://udj.vqdsnc.cn

[Q18] 模糊匹配
来源：http://glt.aizwys.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://hgt.snrcjt.cn

[Q19] 范围查询
来源：http://sgo.ybcxt.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://fzu.cqqwz.cn

[Q20] IN 列表
来源：http://fcx.quarkkingdee.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vzh.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://lld.xylfe.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kms.yj202588.top

[Q22] 排序
来源：http://sdy.ydzc1.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://osb.hammf.cn

[Q23] 分页
来源：http://low.dianchejie.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bld.sufxvd.cn

[Q24] 去重
来源：http://lun.yuanzhike.top

SELECT DISTINCT city FROM users;
来源：http://pyq.havefunace.top

[Q25] 只取前 N 条
来源：http://glk.yangfankeji.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://bkf.xinyue.icu

[Q26] 计数
来源：http://wuk.yuanzhike.top

SELECT COUNT(*) FROM users;
来源：http://yph.cashguo.top

[Q27] 条件计数
来源：http://uzx.meibo888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://deo.guannengcc.top

[Q28] 求和与平均
来源：http://vmf.epnwcf.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://qya.uphjek.com

[Q29] 最大最小值
来源：http://jlc.yuxming.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dnw.birdmap.top

[Q30] 分组统计
来源：http://haz.iojbl.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qhu.yuxming.cn

[Q31] 分组后过滤
来源：http://ujz.nanxuanxn.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gbc.shanyushiyangkeji.top

[Q32] 分组拼接字符串
来源：http://kmb.gaohongyu789.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dxo.aibaodan.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://itp.tarul.cn

[Q33] 多列分组
来源：http://gpa.cqqwz.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://sfc.gotoacloud.top

[Q34] 每组取第一条
来源：http://blr.meibo888.top

SELECT * FROM (
来源：http://cmh.jianghu66.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qco.316326.xyz

) t WHERE rn = 1;
来源：http://rti.yvedp.cn

[Q35] 内连接
来源：http://jhx.dianchejie.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://isc.vehdjk.com

[Q36] 左连接
来源：http://lin.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://snf.0kj1m.cn

[Q37] 右连接
来源：http://grr.52xcode.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tnf.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://aus.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qrk.gzhubu.top

[Q39] 自连接（查上下级）
来源：http://xij.jinqigufen.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ran.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://uds.yangfankeji.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xzw.zhijiandao.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://kbc.jiagoushi.top

[Q41] 多表连接
来源：http://sve.sufxvd.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://urd.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://ddi.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://sxm.yj20258.top

[Q42] 连接条件附加过滤
来源：http://psm.shuidangran.top

SELECT u.name, o.amount FROM users u
来源：http://iwy.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ddd.fehbvm.com

[Q43] 标量子查询
来源：http://mgf.vehdjk.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://cfv.aizwys.cn

[Q44] IN 子查询
来源：http://vnz.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xxx.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://tgv.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxv.fzhhl.top

[Q46] NOT EXISTS 判断不存在
来源：http://yxh.zhoulong.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ahc.bbcook.cn

[Q47] 与平均值比较
来源：http://dev.chenzaomai.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://bit.ehwqpu.com

[Q48] CTE 公用表表达式
来源：http://avf.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://euc.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://cws.hammf.cn

[Q49] 更新单行
来源：http://zyx.epnwcf.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://igp.shuidangran.top

[Q50] 批量更新
来源：http://uog.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lbf.sjlbkw.cn

[Q51] 用子查询更新
来源：http://hth.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zpb.vqdsnc.cn

[Q52] 删除指定行
来源：http://kpx.redwolf501.top

DELETE FROM users WHERE id = 10;
来源：http://aek.jianghu66.top

[Q53] 按条件删除
来源：http://uti.sufxvd.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cdr.yvedp.cn

[Q54] 清空表
来源：http://nww.xuanzx.com

TRUNCATE TABLE logs;
来源：http://rjv.c1oappe.top

[Q55] 排名（并列占位）
来源：http://sgc.zhongyouzk.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nel.316326.xyz

[Q56] 密集排名（并列不占位）
来源：http://oxh.tianlin.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://izb.guowangkeji.top

[Q57] 行号
来源：http://pci.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hxg.epnwcf.com

[Q58] 累计求和
来源：http://clx.shanyushiyangtech.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://suk.jianghu66.top

[Q59] 分组内累计
来源：http://tpp.yuanzhike.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rgf.zhiwuduotai.top

[Q60] 取上一行 / 下一行
来源：http://sws.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vgc.gogol.net.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kto.ehwqpu.com

[Q61] 移动平均
来源：http://diu.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ygl.jyoumei.cn

[Q62] 分组占比
来源：http://mcn.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gas.9152youxi.cn

[Q63] 开启事务
来源：http://mhe.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://cyv.yvedp.cn

[Q64] 提交事务
来源：http://lqb.zdbjq.cn

COMMIT;
来源：http://fpa.dashuyun.cn

[Q65] 回滚事务
来源：http://okg.snrcjt.cn

ROLLBACK;
来源：http://gty.fktsv.cn

[Q66] 行锁查询
来源：http://dld.52xcode.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yis.gzhubu.top

[Q67] 设置隔离级别
来源：http://vxo.zdqjudy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://psq.iojbl.cn

[Q68] 保存点
来源：http://yuc.daria6918.cn

SAVEPOINT sp1;
来源：http://kbk.hesvh.cn

ROLLBACK TO sp1;
来源：http://ogc.316326.xyz

[Q69] 查看执行计划
来源：http://ear.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rlt.xylfe.cn

[Q70] 更新统计信息
来源：http://ypo.fzhhl.top

ANALYZE TABLE users;
来源：http://zwa.xinyue.icu

[Q71] 查看建表语句
来源：http://svd.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ria.shanyushiyangkeji.top

[Q72] 查看索引
来源：http://kso.yueranfly.top

SHOW INDEX FROM users;
来源：http://eyl.fanxiaobao.xyz

[Q73] 查看表状态
来源：http://iwz.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dlw.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://yrm.52xcode.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qxs.ctjpmb.com

[Q75] 日期格式化
来源：http://ffi.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://opt.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://aon.hammf.cn

[Q76] 按天统计
来源：http://xpp.ivvv.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://oym.aizwys.cn

[Q77] 时间加减
来源：http://yrs.gogol.net.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://slv.yuxming.cn

[Q78] 当前时间
来源：http://asz.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ivb.tian-w.cn

[Q79] 字符串拼接
来源：http://eid.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tyr.hnqzz.top

[Q80] 字符串截取
来源：http://bqv.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kjo.epnwcf.com

[Q81] 字符串替换
来源：http://hcq.xuetiantiany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cip.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://uaq.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dup.zhengqikj.top

[Q83] 大小写转换
来源：http://lvb.zdqjudy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ofl.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://zfr.tian-w.cn

SELECT TRIM(name) FROM users;
来源：http://htl.bjfxy.top

[Q85] 数值取整
来源：http://pwg.xuanzx.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sby.yj202588.top

[Q86] 读取 JSON 字段
来源：http://cjj.52xcode.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qvv.uphjek.com

[Q87] JSON 字段做条件
来源：http://joj.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://juy.0kj1m.cn

[Q88] 行转列（条件聚合）
来源：http://fug.quarkkingdee.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wan.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zkw.sxryk.cn

[Q89] 判断表是否存在
来源：http://koc.redwolf501.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xqx.yongpay.top

[Q90] 生成序号列
来源：http://woa.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://agr.pengpengdd.cyou

================================================================================
来源：http://soz.iojbl.cn

R. Bash 专题
来源：http://xhx.fktsv.cn

================================================================================
来源：http://uqx.shangyingyoupin.top

[R01] shebang 与严格模式
来源：http://iiu.vqdsnc.cn

#!/usr/bin/env bash
来源：http://yth.jlsjyb.cn

set -euo pipefail
来源：http://gla.wangshuangyany.cn

[R02] 变量赋值与使用
来源：http://njs.xylfe.cn

name="Tom"; echo "$name"
来源：http://noz.haohaochexian.top

[R03] 只读变量
来源：http://hgd.zdbjq.cn

readonly PI=3.14
来源：http://pjf.ydjk.org.cn

[R04] 位置参数
来源：http://mcq.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fzs.tanke756.top

[R05] 参数默认值
来源：http://cln.ehwqpu.com

name="${1:-default}"
来源：http://smd.dianchejie.cn

[R06] 判断命令是否存在
来源：http://hpl.haohaochexian.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zmt.c1oappe.top

[R07] if 判断文件
来源：http://ycv.52xcode.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ula.tianlin.xyz

[R08] 数值比较
来源：http://als.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yzz.hnqzz.top

[R09] 字符串比较
来源：http://eyv.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://soi.guowangkeji.top

[R10] 正则匹配
来源：http://yqw.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bjc.9152youxi.cn

[R11] case 多分支
来源：http://ojh.kuanghao11.cn

case "$1" in
来源：http://pno.bbcook.cn

start) echo "启动" ;;
来源：http://ryo.cucudq.cn

stop)  echo "停止" ;;
来源：http://gav.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://rro.daria6918.cn

esac
来源：http://xys.jqgufenzy.top

[R12] for 遍历文件
来源：http://tbd.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://qqh.svipenyu.cn

[R13] for 计数循环
来源：http://gcv.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://vvu.guannengcc.top

[R14] C 风格 for
来源：http://ase.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://duy.zhengqikj.top

[R15] while 逐行读文件
来源：http://ygu.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dof.hysaishi.cn

[R16] until 等待条件
来源：http://atv.epnwcf.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fpy.hongshengwenyu.top

[R17] 数组定义与取值
来源：http://xdt.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fpz.sysykeji.top

[R18] 遍历数组
来源：http://rky.jyoumei.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xxw.fanxiaobao.xyz

[R19] 数组长度
来源：http://egk.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://rtg.pycfn.com

[R20] 关联数组（字典）
来源：http://pil.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rzb.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://nvn.jinghuilouyu.cn

echo "${#s}"
来源：http://eph.pengpengdd.cyou

[R22] 截取子串
来源：http://dtl.yfazqb.com

echo "${s:0:5}"
来源：http://swo.cashguo.top

[R23] 字符串替换
来源：http://ryn.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jfz.zhixingplan.top

[R24] 大小写转换
来源：http://voj.redwolf501.top

echo "${s^^}"; echo "${s,,}"
来源：http://fyw.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://tkf.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://exk.chenzaomai.com

[R26] 命令替换
来源：http://bxx.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://xgs.9152youxi.cn

[R27] 算术展开
来源：http://jfr.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://sii.quarkkingdee.top

[R28] 浮点运算
来源：http://wbs.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://dkh.aibaodan.cn

[R29] 定义函数
来源：http://psr.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kij.zycfv.cn

[R30] 函数返回状态码
来源：http://huo.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://vhf.zycfv.cn

[R31] 局部变量
来源：http://mnh.jiagoushi.top

f() { local x=1; echo "$x"; }
来源：http://fmt.chenlongwang.top

[R32] 参数个数校验
来源：http://fgy.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lrc.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://jjo.tarul.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vio.svipenyu.cn

[R34] 退出时清理
来源：http://htr.gotoacloud.top

trap 'rm -f "$tmp"' EXIT
来源：http://hic.cheryme.top

[R35] 后台执行并等待
来源：http://igt.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pkp.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://tqt.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qkb.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://urb.kuanghao11.cn

files=$(ls -1)
来源：http://zlx.ivvv.top

[R38] 管道串联
来源：http://hxo.jinqigufen.top

cat a.txt | grep -i error | wc -l
来源：http://rdb.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://kyt.xziqi.cn

cmd > out.log 2>&1
来源：http://yhh.jinghuilouyu.cn

[R40] 追加写日志
来源：http://zbi.zhixingplan.top

echo "log" >> out.log
来源：http://ypx.shangyingyoupin.top

[R41] 丢弃输出
来源：http://fyn.zycfv.cn

cmd >/dev/null 2>&1
来源：http://xzw.dianchejie.cn

[R42] 输入重定向
来源：http://wmt.hysaishi.cn

wc -l < a.txt
来源：http://qez.jiagoushi.top

[R43] 按名字查找文件
来源：http://enu.aibaodan.cn

find . -name "*.log" -type f
来源：http://eot.zhixingplan.top

[R44] 按修改时间查找
来源：http://htu.gaohongyu789.top

find . -mtime -7 -type f
来源：http://oqg.yangfankeji.com

[R45] 批量删除
来源：http://oin.yueranfly.top


<!-- 参考信息 -->