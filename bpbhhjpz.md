代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://gob.quarkkingdee.top

PHP:  bcadd("0.1", "0.2", 2);
来源：http://rrd.fzhhl.top

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://bgo.52xcode.cn

TS:   (0.1 + 0.2).toFixed(2)
来源：http://ijv.xinyue.icu

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://sye.fanxiaobao.xyz

Go:   math/big.Float，或全部换算成整数分再算
来源：http://utg.yfazqb.com

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://dre.hysaishi.cn

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://ecb.pycfn.com

================================================================================
来源：http://six.sufxvd.cn

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mvq.dianchejie.cn

================================================================================
来源：http://llj.yongpay.top

[Q01] 创建表
来源：http://wgk.redwolf501.top

CREATE TABLE users (
来源：http://rij.shanyushiyangkeji.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://bwf.jqgfzy.top

name VARCHAR(50) NOT NULL,
来源：http://wrm.316326.xyz

email VARCHAR(100) UNIQUE,
来源：http://xrs.tianlin.xyz

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://uxa.redwolf501.top

);
来源：http://lmi.hongshengwenyu.top

[Q02] 创建带外键的表
来源：http://nxf.c1oappe.top

CREATE TABLE orders (
来源：http://fjl.chenzaomai.com

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://nes.hnxiangtu.top

user_id INT NOT NULL,
来源：http://dnv.c1oappe.top

amount DECIMAL(10, 2),
来源：http://fuq.sysykeji.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gzc.yangfankeji.com

);
来源：http://rpx.fanxiaobao.xyz

[Q03] 增加列
来源：http://tbu.hnqzz.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://azb.redwolf501.top

[Q04] 修改列类型
来源：http://jlt.feifeiyinyue.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nfq.dianchejie.cn

[Q05] 重命名列
来源：http://edq.nwbrower.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hfv.bjfxy.top

[Q06] 删除列
来源：http://ain.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://njm.nanxuanxn.top

[Q07] 删除表
来源：http://ghu.zhongyouzk.top

DROP TABLE IF EXISTS orders;
来源：http://ldr.yangfankeji.com

[Q08] 创建普通索引
来源：http://lja.sxryk.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hbz.ybcxt.top

[Q09] 创建唯一索引
来源：http://cro.smart0.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://two.zdqjudy.top

[Q10] 插入单行
来源：http://yvv.nanxuanxn.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://jfa.9152youxi.cn

[Q11] 一次插入多行
来源：http://lvp.shzxlz.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rio.jinyuanbaomall.cn

[Q12] 插入后取自增 ID
来源：http://oui.c1oappe.top

INSERT INTO users (name) VALUES ('C');
来源：http://uzi.shangyingyoupin.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wwq.shuidangran.top

[Q13] 忽略重复插入
来源：http://kuy.zdqjudy.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://fap.9152youxi.cn

[Q14] 存在则更新（upsert）
来源：http://wrc.jyoumei.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rdt.nanxuanxn.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://uwa.feifeiyinyue.top

[Q15] 查询全部
来源：http://auj.sxryk.cn

SELECT * FROM users;
来源：http://cbb.ivvv.top

[Q16] 查询指定列
来源：http://sdx.bbcook.cn

SELECT id, name FROM users;
来源：http://ztt.ivvv.top

[Q17] 条件查询
来源：http://saz.cqqwz.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://znu.ydjk.org.cn

[Q18] 模糊匹配
来源：http://nil.nwbrower.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://nfj.andypj.xyz

[Q19] 范围查询
来源：http://lax.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ujm.sweek.top

[Q20] IN 列表
来源：http://iwy.yuanzhike.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ytt.mhx1999.top

[Q21] 空值判断
来源：http://nmn.smart0.xyz

SELECT * FROM users WHERE email IS NULL;
来源：http://fuo.xuetiantiany.cn

[Q22] 排序
来源：http://wgf.aizwys.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zto.yonumen.top

[Q23] 分页
来源：http://pzj.gaohongyu789.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://zip.yj202588.top

[Q24] 去重
来源：http://sml.ywan-chungtsiang.top

SELECT DISTINCT city FROM users;
来源：http://svf.sweek.top

[Q25] 只取前 N 条
来源：http://yri.jinyuanbaomall.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://iuq.cdnleiting.top

[Q26] 计数
来源：http://mya.ydjk.org.cn

SELECT COUNT(*) FROM users;
来源：http://ztc.52xcode.cn

[Q27] 条件计数
来源：http://lnd.gzhubu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://pur.ydjk.org.cn

[Q28] 求和与平均
来源：http://rzk.xziqi.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pkk.xuetiantiany.cn

[Q29] 最大最小值
来源：http://evj.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://ccg.ivvv.top

[Q30] 分组统计
来源：http://zoq.zhengqikj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vue.yj20258.top

[Q31] 分组后过滤
来源：http://xrt.gotoacloud.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ljf.gogol.net.cn

[Q32] 分组拼接字符串
来源：http://fpp.ctjpmb.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ded.fengsongda.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://nmk.birdmap.top

[Q33] 多列分组
来源：http://bma.jiagoushi.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cpo.zhengqikj.top

[Q34] 每组取第一条
来源：http://tuh.aibaodan.cn

SELECT * FROM (
来源：http://vge.fzhhl.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lde.jqgufenzy.top

) t WHERE rn = 1;
来源：http://ynk.xuanzx.com

[Q35] 内连接
来源：http://nsl.yonumen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qkg.fengsongda.top

[Q36] 左连接
来源：http://ufm.hcnkem.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cku.fengsongda.top

[Q37] 右连接
来源：http://zdi.9152youxi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://aee.redwolf501.top

[Q38] 全外连接（PostgreSQL）
来源：http://ceq.meibo888.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hoa.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://jef.cqqwz.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://khb.zhixingplan.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mkm.guannengcc.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pjh.zhaomingkeji.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wbm.zhijiandao.cn

[Q41] 多表连接
来源：http://zgu.pycfn.com

SELECT o.id, u.name, p.title FROM orders o
来源：http://pyv.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://tpo.hywenlv.cn

JOIN products p ON p.id = o.product_id;
来源：http://sxp.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://kqr.sufxvd.cn

SELECT u.name, o.amount FROM users u
来源：http://axc.guowangkeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ktz.cdnleiting.top

[Q43] 标量子查询
来源：http://ybh.daria6918.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://non.xuanzx.com

[Q44] IN 子查询
来源：http://nlx.tarul.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tkz.birdmap.top

[Q45] EXISTS 判断存在
来源：http://zzx.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zwk.xuanzx.com

[Q46] NOT EXISTS 判断不存在
来源：http://npv.shuidangran.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bwb.wangshuangyany.cn

[Q47] 与平均值比较
来源：http://ycy.jinyuanbaomall.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://shc.chenlongwang.top

[Q48] CTE 公用表表达式
来源：http://cxo.cucudq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ftr.meibo888.top

SELECT * FROM t WHERE c > 5;
来源：http://jas.shanyushiyangtech.top

[Q49] 更新单行
来源：http://jsc.cqqwz.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://epu.316326.xyz

[Q50] 批量更新
来源：http://qaj.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bks.sjlbkw.cn

[Q51] 用子查询更新
来源：http://snb.daxiang520.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rgm.zhiwuduotai.top

[Q52] 删除指定行
来源：http://kzj.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://qbd.jyoumei.cn

[Q53] 按条件删除
来源：http://pxp.daria6918.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tfo.hywenlv.cn

[Q54] 清空表
来源：http://qig.yj20258.top

TRUNCATE TABLE logs;
来源：http://fri.wangdashe.top

[Q55] 排名（并列占位）
来源：http://rtu.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gsx.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://uch.zhoulong.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bgn.zhixingplan.top

[Q57] 行号
来源：http://epb.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://igf.fengsongda.top

[Q58] 累计求和
来源：http://txi.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pwi.gotoacloud.top

[Q59] 分组内累计
来源：http://zjv.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sge.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://mzg.ybcxt.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kxs.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://btj.wangshuangyany.cn

[Q61] 移动平均
来源：http://nrs.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bkm.yfazqb.com

[Q62] 分组占比
来源：http://dqg.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ebk.fktsv.cn

[Q63] 开启事务
来源：http://srt.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://grk.zdbjq.cn

[Q64] 提交事务
来源：http://pup.haohaochexian.top

COMMIT;
来源：http://fnc.fanxiaobao.xyz

[Q65] 回滚事务
来源：http://iga.quarkkingdee.top

ROLLBACK;
来源：http://oez.hnqzz.top

[Q66] 行锁查询
来源：http://wne.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://flr.shuidangran.top

[Q67] 设置隔离级别
来源：http://eyf.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dcd.xylfe.cn

[Q68] 保存点
来源：http://nxt.zhijiandao.cn

SAVEPOINT sp1;
来源：http://lvk.tarul.cn

ROLLBACK TO sp1;
来源：http://fdr.sufxvd.cn

[Q69] 查看执行计划
来源：http://ayp.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jgo.iojbl.cn

[Q70] 更新统计信息
来源：http://ptm.chenzaomai.com

ANALYZE TABLE users;
来源：http://zma.hammf.cn

[Q71] 查看建表语句
来源：http://qub.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://toa.fanxiaobao.xyz

[Q72] 查看索引
来源：http://gqk.hfpthk.cn

SHOW INDEX FROM users;
来源：http://lwj.uphjek.com

[Q73] 查看表状态
来源：http://iwe.52xcode.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lut.gogol.net.cn

[Q74] 强制使用索引
来源：http://ecu.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tfu.zhoulong.xyz

[Q75] 日期格式化
来源：http://tfd.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hmn.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://sww.guowangkeji.top

[Q76] 按天统计
来源：http://clu.sjlbkw.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://crb.jqgfzy.top

[Q77] 时间加减
来源：http://ljn.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ddc.nanxuanxn.top

[Q78] 当前时间
来源：http://drj.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ldb.zhengqikj.top

[Q79] 字符串拼接
来源：http://cxv.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://srd.yueranfly.top

[Q80] 字符串截取
来源：http://nni.shzxlz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://owa.fzhhl.top

[Q81] 字符串替换
来源：http://nbv.shzxlz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://adi.meibo888.top

[Q82] 字符长度与字节长度
来源：http://dxo.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mvs.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://cxq.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nhy.jlsjyb.cn

[Q84] 去除首尾空格
来源：http://rus.xuetiantiany.cn

SELECT TRIM(name) FROM users;
来源：http://ekx.dianchejie.cn

[Q85] 数值取整
来源：http://fwl.nanxinkj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://uwh.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://yol.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rne.hesvh.cn

[Q87] JSON 字段做条件
来源：http://qer.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://osb.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://noc.hcnkem.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mwo.jlsjyb.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ymz.andypj.xyz

[Q89] 判断表是否存在
来源：http://bmc.aibaodan.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xpa.gogol.net.cn

[Q90] 生成序号列
来源：http://kyk.ppjwa.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uza.yuxming.cn

================================================================================
来源：http://glp.dashuyun.cn

R. Bash 专题
来源：http://ozc.yangfankeji.com

================================================================================
来源：http://kwb.bbcook.cn

[R01] shebang 与严格模式
来源：http://jgp.jinqigfzy.top

#!/usr/bin/env bash
来源：http://nug.gotoacloud.top

set -euo pipefail
来源：http://vjr.ywan-chungtsiang.top

[R02] 变量赋值与使用
来源：http://uwo.hongshengwenyu.top

name="Tom"; echo "$name"
来源：http://miz.cashguo.top

[R03] 只读变量
来源：http://bog.guowangkeji.top

readonly PI=3.14
来源：http://yto.cashguo.top

[R04] 位置参数
来源：http://bpj.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fne.yvedp.cn

[R05] 参数默认值
来源：http://nva.mhx1999.top

name="${1:-default}"
来源：http://rll.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://dyr.chenzaomai.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wmb.0kj1m.cn

[R07] if 判断文件
来源：http://may.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ptz.quarkkingdee.top

[R08] 数值比较
来源：http://jdy.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pkt.hongshengwenyu.top

[R09] 字符串比较
来源：http://xao.redwolf501.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nxb.hammf.cn

[R10] 正则匹配
来源：http://uxg.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qwi.quarkkingdee.top

[R11] case 多分支
来源：http://tmo.zycfv.cn

case "$1" in
来源：http://zqt.zhongyouzk.top

start) echo "启动" ;;
来源：http://tis.zhixingplan.top

stop)  echo "停止" ;;
来源：http://bjn.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://kpx.ctjpmb.com

esac
来源：http://kyn.fzhhl.top

[R12] for 遍历文件
来源：http://ohf.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://rxx.xuanzx.com

[R13] for 计数循环
来源：http://cnd.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://xaa.hysaishi.cn

[R14] C 风格 for
来源：http://vyl.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ngh.tarul.cn

[R15] while 逐行读文件
来源：http://mqi.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xrq.uphjek.com

[R16] until 等待条件
来源：http://cbj.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uto.tianlin.xyz

[R17] 数组定义与取值
来源：http://lzc.uphjek.com

arr=(a b c); echo "${arr[0]}"
来源：http://vuh.wangdashe.top

[R18] 遍历数组
来源：http://sld.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qtt.ctjpmb.com

[R19] 数组长度
来源：http://ufi.aibaodan.cn

echo "${#arr[@]}"
来源：http://hsr.meibo888.top

[R20] 关联数组（字典）
来源：http://fdr.xylfe.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://axa.haohaochexian.top

[R21] 字符串长度
来源：http://aig.cqqwz.cn

echo "${#s}"
来源：http://qfc.tanke756.top

[R22] 截取子串
来源：http://vhw.dashuyun.cn

echo "${s:0:5}"
来源：http://aru.gaohongyu789.top

[R23] 字符串替换
来源：http://fhd.bjfxy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ujs.hammf.cn

[R24] 大小写转换
来源：http://tnt.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://dpu.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://wsq.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://dbz.cheryme.top

[R26] 命令替换
来源：http://doh.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://xtm.hfpthk.cn

[R27] 算术展开
来源：http://uwr.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://pzp.yj20258888.top

[R28] 浮点运算
来源：http://jgk.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://oqn.ehwqpu.com

[R29] 定义函数
来源：http://xhe.iojbl.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uqh.sxryk.cn

[R30] 函数返回状态码
来源：http://evh.sjlbkw.cn

f() { return 0; }; f || echo "失败了"
来源：http://axb.shangyingyoupin.top

[R31] 局部变量
来源：http://gix.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://fjc.sysykeji.top

[R32] 参数个数校验
来源：http://luq.jianghu66.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://szf.kuanghao11.cn

[R33] 捕获错误并提示行号
来源：http://rhr.xuanzx.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xzi.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://pqt.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://scf.yj202588.top

[R35] 后台执行并等待
来源：http://rcq.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ehe.svipenyu.cn

[R36] 并发执行多个任务
来源：http://djf.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pae.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://ocp.chenjidiqi.icu

files=$(ls -1)
来源：http://tmn.ppjwa.cn

[R38] 管道串联
来源：http://wqj.dianchejie.cn

cat a.txt | grep -i error | wc -l
来源：http://ysk.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://jhe.ehwqpu.com


<!-- 参考信息 -->