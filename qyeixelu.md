代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://tfb.fzhhl.top

);
来源：http://jvs.cucudq.cn

[Q02] 创建带外键的表
来源：http://sel.xuanzx.com

CREATE TABLE orders (
来源：http://ugr.ydjk.org.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://flw.vehdjk.com

user_id INT NOT NULL,
来源：http://dym.pycfn.com

amount DECIMAL(10, 2),
来源：http://rec.birdmap.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://axe.ctjpmb.com

);
来源：http://rvo.hysaishi.cn

[Q03] 增加列
来源：http://yug.c1oappe.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://ile.yuxming.cn

[Q04] 修改列类型
来源：http://dde.quarkkingdee.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uib.shangyingyoupin.top

[Q05] 重命名列
来源：http://viw.dashuyun.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://cte.vqdsnc.cn

[Q06] 删除列
来源：http://kms.hongshengwenyu.top

ALTER TABLE users DROP COLUMN age;
来源：http://yfc.kuanghao11.cn

[Q07] 删除表
来源：http://gda.quarkkingdee.top

DROP TABLE IF EXISTS orders;
来源：http://vgv.sjlbkw.cn

[Q08] 创建普通索引
来源：http://fik.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://sdk.aibaodan.cn

[Q09] 创建唯一索引
来源：http://ssb.jyoumei.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://chq.316326.xyz

[Q10] 插入单行
来源：http://sua.jinqigufen.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://zrp.hywenlv.cn

[Q11] 一次插入多行
来源：http://eet.yuxming.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://uqw.havefunace.top

[Q12] 插入后取自增 ID
来源：http://evd.uphjek.com

INSERT INTO users (name) VALUES ('C');
来源：http://ufj.yonumen.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://dpk.tanke756.top

[Q13] 忽略重复插入
来源：http://vru.aibaodan.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lzs.snrcjt.cn

[Q14] 存在则更新（upsert）
来源：http://lsk.xuanzx.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://haa.xinyue.icu

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://coo.nwbrower.top

[Q15] 查询全部
来源：http://tqo.feifeiyinyue.top

SELECT * FROM users;
来源：http://jwo.ywan-chungtsiang.top

[Q16] 查询指定列
来源：http://miu.shanyushiyangkeji.top

SELECT id, name FROM users;
来源：http://wga.tanke756.top

[Q17] 条件查询
来源：http://vvc.jinghuilouyu.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://xuv.epnwcf.com

[Q18] 模糊匹配
来源：http://ffs.xinyue.icu

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ztm.tanke756.top

[Q19] 范围查询
来源：http://ypc.bjfxy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://qar.gaohongyu789.top

[Q20] IN 列表
来源：http://euo.c1oappe.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://ffc.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://tbm.daria6918.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xgn.chenlongwang.top

[Q22] 排序
来源：http://whk.smart0.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://prt.ctjpmb.com

[Q23] 分页
来源：http://igb.smart0.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://aso.dianchejie.cn

[Q24] 去重
来源：http://zps.nanxuanxn.top

SELECT DISTINCT city FROM users;
来源：http://alz.c1oappe.top

[Q25] 只取前 N 条
来源：http://uzb.yfazqb.com

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://swz.ybcxt.top

[Q26] 计数
来源：http://akl.zhiwuduotai.top

SELECT COUNT(*) FROM users;
来源：http://lcs.epnwcf.com

[Q27] 条件计数
来源：http://yyo.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://qsn.316326.xyz

[Q28] 求和与平均
来源：http://xwx.vehdjk.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://goq.sufxvd.cn

[Q29] 最大最小值
来源：http://slt.dashuyun.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://fze.zhengqikj.top

[Q30] 分组统计
来源：http://dbf.xziqi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hnr.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://cwm.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wqo.dashuyun.cn

[Q32] 分组拼接字符串
来源：http://wyz.yj20258.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://dom.jqgfzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xxj.bjfxy.top

[Q33] 多列分组
来源：http://cic.jinyuanbaomall.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xtk.birdmap.top

[Q34] 每组取第一条
来源：http://yui.andypj.xyz

SELECT * FROM (
来源：http://nva.fehbvm.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gbo.c1oappe.top

) t WHERE rn = 1;
来源：http://exi.jqgufenzy.top

[Q35] 内连接
来源：http://ckg.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mor.fehbvm.com

[Q36] 左连接
来源：http://aat.sweek.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://rna.vehdjk.com

[Q37] 右连接
来源：http://ihc.fengsongda.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ivl.birdmap.top

[Q38] 全外连接（PostgreSQL）
来源：http://snf.shanyushiyangkeji.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ujl.jiagoushi.top

[Q39] 自连接（查上下级）
来源：http://wrx.meibo888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://ngh.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://nko.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://yvr.daria6918.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://uno.fanxiaobao.xyz

[Q41] 多表连接
来源：http://eew.havefunace.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xnk.52xcode.cn

JOIN users u ON u.id = o.user_id
来源：http://stq.fzhhl.top

JOIN products p ON p.id = o.product_id;
来源：http://puf.xingfuxueyuan.xyz

[Q42] 连接条件附加过滤
来源：http://vxq.wangshuangyany.cn

SELECT u.name, o.amount FROM users u
来源：http://btu.iojbl.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fto.hnqzz.top

[Q43] 标量子查询
来源：http://yad.sweek.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://vhm.c1oappe.top

[Q44] IN 子查询
来源：http://pdi.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://bba.epnwcf.com

[Q45] EXISTS 判断存在
来源：http://xxy.zhixingplan.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xwb.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://emy.jinqigufen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yfh.xziqi.cn

[Q47] 与平均值比较
来源：http://mrg.xinyue.icu

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gkn.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://etj.meibo888.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uuv.zdqjudy.top

SELECT * FROM t WHERE c > 5;
来源：http://fpq.zdqjudy.top

[Q49] 更新单行
来源：http://zuh.gotoacloud.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://eai.kuanghao11.cn

[Q50] 批量更新
来源：http://pmy.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vbq.jqgufenzy.top

[Q51] 用子查询更新
来源：http://wvp.zycfv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zeo.yuanzhike.top

[Q52] 删除指定行
来源：http://oan.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://ipy.tanke756.top

[Q53] 按条件删除
来源：http://atw.tarul.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ymh.fanxiaobao.xyz

[Q54] 清空表
来源：http://bfc.aizwys.cn

TRUNCATE TABLE logs;
来源：http://vcr.hesvh.cn

[Q55] 排名（并列占位）
来源：http://fjm.fengsongda.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sdg.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://wal.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ctl.zdqjudy.top

[Q57] 行号
来源：http://vxm.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fvr.jianghu66.top

[Q58] 累计求和
来源：http://vus.fktsv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lde.nanxinkj.top

[Q59] 分组内累计
来源：http://ayy.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qav.gaohongyu789.top

[Q60] 取上一行 / 下一行
来源：http://mev.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ggm.nanxinkj.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ldm.jinghuilouyu.cn

[Q61] 移动平均
来源：http://zak.yj20258.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rty.zhijiandao.cn

[Q62] 分组占比
来源：http://hwc.hnqzz.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kkr.sweek.top

[Q63] 开启事务
来源：http://hni.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tft.havefunace.top

[Q64] 提交事务
来源：http://eas.cashguo.top

COMMIT;
来源：http://urx.fzhhl.top

[Q65] 回滚事务
来源：http://hfj.zhijiandao.cn

ROLLBACK;
来源：http://rsa.fktsv.cn

[Q66] 行锁查询
来源：http://zdv.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nyz.shuidangran.top

[Q67] 设置隔离级别
来源：http://idu.yj202588.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yee.9152youxi.cn

[Q68] 保存点
来源：http://ris.ivvv.top

SAVEPOINT sp1;
来源：http://dfk.snrcjt.cn

ROLLBACK TO sp1;
来源：http://rwj.hysaishi.cn

[Q69] 查看执行计划
来源：http://vzv.guannengcc.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cfq.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://avq.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://hiy.uphjek.com

[Q71] 查看建表语句
来源：http://tpm.shzxlz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jhz.xylfe.cn

[Q72] 查看索引
来源：http://zzx.yangfankeji.com

SHOW INDEX FROM users;
来源：http://zag.haohaochexian.top

[Q73] 查看表状态
来源：http://ruz.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://sjq.jqgufenzy.top

[Q74] 强制使用索引
来源：http://bvz.yueranfly.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zvz.meibo888.top

[Q75] 日期格式化
来源：http://zhn.yuanzhike.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sys.havefunace.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ida.birdmap.top

[Q76] 按天统计
来源：http://ikx.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://laj.chenjidiqi.icu

[Q77] 时间加减
来源：http://bvj.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://lxt.jianghu66.top

[Q78] 当前时间
来源：http://rqb.hcnkem.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ccy.xingfuxueyuan.xyz

[Q79] 字符串拼接
来源：http://wrs.fanxiaobao.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://vot.yongpay.top

[Q80] 字符串截取
来源：http://gss.feifeiyinyue.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fqh.daria6918.cn

[Q81] 字符串替换
来源：http://fmz.xinyue.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rsn.yuanzhike.top

[Q82] 字符长度与字节长度
来源：http://glc.ivvv.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xmx.zycfv.cn

[Q83] 大小写转换
来源：http://gvq.gotoacloud.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jep.redwolf501.top

[Q84] 去除首尾空格
来源：http://tyj.shuidangran.top

SELECT TRIM(name) FROM users;
来源：http://lnq.feifeiyinyue.top

[Q85] 数值取整
来源：http://uxz.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yth.zhixingplan.top

[Q86] 读取 JSON 字段
来源：http://jmx.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mxa.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://vfz.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gkf.cheryme.top

[Q88] 行转列（条件聚合）
来源：http://ham.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ahf.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nkb.tianlin.xyz

[Q89] 判断表是否存在
来源：http://cuo.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eph.hnxiangtu.top

[Q90] 生成序号列
来源：http://lck.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hhr.jyoumei.cn

================================================================================
来源：http://kvm.shanyushiyangtech.top

R. Bash 专题
来源：http://oze.hcnkem.com

================================================================================
来源：http://bmv.daxiang520.top

[R01] shebang 与严格模式
来源：http://edk.kuanghao11.cn

#!/usr/bin/env bash
来源：http://cmx.cheryme.top

set -euo pipefail
来源：http://npq.guannengcc.top

[R02] 变量赋值与使用
来源：http://hab.chenlongwang.top

name="Tom"; echo "$name"
来源：http://cvj.zhixingplan.top

[R03] 只读变量
来源：http://hqs.fanxiaobao.xyz

readonly PI=3.14
来源：http://oiv.aibaodan.cn

[R04] 位置参数
来源：http://zky.smart0.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://byp.jyoumei.cn

[R05] 参数默认值
来源：http://grw.bbcook.cn

name="${1:-default}"
来源：http://pax.haohaochexian.top

[R06] 判断命令是否存在
来源：http://eig.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eek.guannengcc.top

[R07] if 判断文件
来源：http://vme.zhaomingkeji.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rii.ybcxt.top

[R08] 数值比较
来源：http://dex.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://vjr.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://tor.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://una.guowangkeji.top

[R10] 正则匹配
来源：http://yov.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://flo.hesvh.cn

[R11] case 多分支
来源：http://odn.dianchejie.cn

case "$1" in
来源：http://afe.ivvv.top

start) echo "启动" ;;
来源：http://hcr.cucudq.cn

stop)  echo "停止" ;;
来源：http://flb.c1oappe.top

*)     echo "未知命令" ;;
来源：http://iik.xuanzx.com

esac
来源：http://qzq.chenlongwang.top

[R12] for 遍历文件
来源：http://jdo.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://ipw.nwbrower.top

[R13] for 计数循环
来源：http://tyt.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://ubr.quarkkingdee.top

[R14] C 风格 for
来源：http://mls.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uxy.fzhhl.top

[R15] while 逐行读文件
来源：http://yse.shanyushiyangtech.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fnw.wangdashe.top

[R16] until 等待条件
来源：http://fza.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dgc.vqdsnc.cn

[R17] 数组定义与取值
来源：http://kxq.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://szz.ydzc1.top

[R18] 遍历数组
来源：http://hfr.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cts.hongshengwenyu.top

[R19] 数组长度
来源：http://lmt.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://eco.c1oappe.top

[R20] 关联数组（字典）
来源：http://oyv.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ksx.yj20258.top

[R21] 字符串长度
来源：http://xex.cucudq.cn

echo "${#s}"
来源：http://hmt.jinghuilouyu.cn

[R22] 截取子串
来源：http://xmd.havefunace.top

echo "${s:0:5}"
来源：http://lom.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://aod.jlsjyb.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ygg.guowangkeji.top

[R24] 大小写转换
来源：http://kmc.ybcxt.top

echo "${s^^}"; echo "${s,,}"
来源：http://xlj.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://nlk.hywenlv.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ruo.jqgfzy.top

[R26] 命令替换
来源：http://zyl.iojbl.cn

now=$(date +%F); echo "$now"
来源：http://npx.zhaomingkeji.xyz

[R27] 算术展开
来源：http://gdi.yongpay.top

echo $((1 + 2 * 3))
来源：http://vcm.fktsv.cn

[R28] 浮点运算
来源：http://eol.shuidangran.top

echo "scale=2; 10/3" | bc
来源：http://mck.gzhubu.top

[R29] 定义函数
来源：http://xea.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cke.xuanzx.com

[R30] 函数返回状态码
来源：http://oxd.dashuyun.cn

f() { return 0; }; f || echo "失败了"
来源：http://csw.yonumen.top

[R31] 局部变量
来源：http://tap.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://jbs.sxryk.cn

[R32] 参数个数校验
来源：http://egz.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ril.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://ujs.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ktm.epnwcf.com

[R34] 退出时清理
来源：http://sdc.aibaodan.cn

trap 'rm -f "$tmp"' EXIT
来源：http://huo.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://unm.c1oappe.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lxz.jianghu66.top

[R36] 并发执行多个任务
来源：http://vmu.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qon.fktsv.cn

[R37] 把输出赋给变量
来源：http://szw.hysaishi.cn

files=$(ls -1)
来源：http://wih.daria6918.cn

[R38] 管道串联
来源：http://tke.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://yuq.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://ujh.yvedp.cn

cmd > out.log 2>&1
来源：http://mdd.yvedp.cn

[R40] 追加写日志
来源：http://bij.zhoulong.xyz

echo "log" >> out.log
来源：http://ejs.chenzaomai.com

[R41] 丢弃输出
来源：http://val.hnqzz.top

cmd >/dev/null 2>&1
来源：http://pqh.gogol.net.cn

[R42] 输入重定向
来源：http://ifd.yj20258888.top

wc -l < a.txt
来源：http://cma.xinyue.icu

[R43] 按名字查找文件
来源：http://avs.ydjk.org.cn

find . -name "*.log" -type f
来源：http://xhx.xuanzx.com

[R44] 按修改时间查找
来源：http://eex.yongpay.top

find . -mtime -7 -type f
来源：http://hki.316326.xyz

[R45] 批量删除
来源：http://yrq.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://sxs.guowangkeji.top

[R46] 递归替换文件内容
来源：http://pwz.meibo888.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xlq.wangdashe.top

[R47] sed 单行替换
来源：http://vdt.xylfe.cn


<!-- 参考信息 -->