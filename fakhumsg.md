代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://vmw.cheryme.top

);
来源：http://esz.zdqjudy.top

[Q02] 创建带外键的表
来源：http://hfo.cashguo.top

CREATE TABLE orders (
来源：http://ymy.iojbl.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://zek.yuxming.cn

user_id INT NOT NULL,
来源：http://gzi.yuxming.cn

amount DECIMAL(10, 2),
来源：http://ozw.jlsjyb.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://bmh.bjfxy.top

);
来源：http://apl.sxryk.cn

[Q03] 增加列
来源：http://vcw.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://mwq.smart0.xyz

[Q04] 修改列类型
来源：http://qje.xziqi.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://bpl.jianghu66.top

[Q05] 重命名列
来源：http://fdu.yanxiufei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://rmi.yangfankeji.com

[Q06] 删除列
来源：http://nxo.aizwys.cn

ALTER TABLE users DROP COLUMN age;
来源：http://vcr.vqdsnc.cn

[Q07] 删除表
来源：http://cws.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://yzo.feifeiyinyue.top

[Q08] 创建普通索引
来源：http://aeu.tian-w.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://hhe.aibaodan.cn

[Q09] 创建唯一索引
来源：http://nex.fanxiaobao.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ahy.snrcjt.cn

[Q10] 插入单行
来源：http://vna.dashuyun.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://rpb.yonumen.top

[Q11] 一次插入多行
来源：http://nbx.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://kto.ctjpmb.com

[Q12] 插入后取自增 ID
来源：http://jdl.svipenyu.cn

INSERT INTO users (name) VALUES ('C');
来源：http://erm.quarkkingdee.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://xxa.hammf.cn

[Q13] 忽略重复插入
来源：http://ncu.feifeiyinyue.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://way.yj20258.top

[Q14] 存在则更新（upsert）
来源：http://gzt.pycfn.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rik.kuanghao11.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wco.vqdsnc.cn

[Q15] 查询全部
来源：http://yiz.ybcxt.top

SELECT * FROM users;
来源：http://kep.yanxiufei.cn

[Q16] 查询指定列
来源：http://rll.shuidangran.top

SELECT id, name FROM users;
来源：http://zqd.chenlongwang.top

[Q17] 条件查询
来源：http://huf.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dnk.dashuyun.cn

[Q18] 模糊匹配
来源：http://ukz.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://kic.xinyue.icu

[Q19] 范围查询
来源：http://huz.pengpengdd.cyou

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://syp.xylfe.cn

[Q20] IN 列表
来源：http://xfd.sweek.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://tco.zhoulong.xyz

[Q21] 空值判断
来源：http://ble.hongshengwenyu.top

SELECT * FROM users WHERE email IS NULL;
来源：http://tsc.vehdjk.com

[Q22] 排序
来源：http://zjw.dashuyun.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qsb.jinqigfzy.top

[Q23] 分页
来源：http://wgp.0kj1m.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://yly.mhx1999.top

[Q24] 去重
来源：http://dpq.0kj1m.cn

SELECT DISTINCT city FROM users;
来源：http://wod.snrcjt.cn

[Q25] 只取前 N 条
来源：http://zzg.andypj.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mss.ybcxt.top

[Q26] 计数
来源：http://kqi.ehwqpu.com

SELECT COUNT(*) FROM users;
来源：http://avb.yuanzhike.top

[Q27] 条件计数
来源：http://emv.svipenyu.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hkr.nanxuanxn.top

[Q28] 求和与平均
来源：http://zev.nwbrower.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://slk.zhixingplan.top

[Q29] 最大最小值
来源：http://bxe.chenlongwang.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://ftp.hammf.cn

[Q30] 分组统计
来源：http://ync.svipenyu.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vya.jqgufenzy.top

[Q31] 分组后过滤
来源：http://dot.smart0.xyz

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://maa.ydzc1.top

[Q32] 分组拼接字符串
来源：http://vig.tian-w.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://epj.zhongyouzk.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ufl.aizwys.cn

[Q33] 多列分组
来源：http://vfh.daria6918.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://zqk.bjfxy.top

[Q34] 每组取第一条
来源：http://eop.hywenlv.cn

SELECT * FROM (
来源：http://sik.tian-w.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xpm.birdmap.top

) t WHERE rn = 1;
来源：http://ied.shzxlz.cn

[Q35] 内连接
来源：http://gxk.xziqi.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://tvw.c1oappe.top

[Q36] 左连接
来源：http://hai.gzhubu.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://emz.yangfankeji.com

[Q37] 右连接
来源：http://ssf.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gya.hcnkem.com

[Q38] 全外连接（PostgreSQL）
来源：http://ofn.svipenyu.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mdm.ydzc1.top

[Q39] 自连接（查上下级）
来源：http://kcp.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://uzz.havefunace.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ano.pycfn.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xkh.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bmh.xziqi.cn

[Q41] 多表连接
来源：http://lqe.redwolf501.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://mkf.ivvv.top

JOIN users u ON u.id = o.user_id
来源：http://byj.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://pbz.xinyue.icu

[Q42] 连接条件附加过滤
来源：http://ntn.zhijiandao.cn

SELECT u.name, o.amount FROM users u
来源：http://fhc.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dvk.gaohongyu789.top

[Q43] 标量子查询
来源：http://hts.sjlbkw.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kok.sufxvd.cn

[Q44] IN 子查询
来源：http://ays.ybcxt.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dab.xuetiantiany.cn

[Q45] EXISTS 判断存在
来源：http://ynm.yongpay.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wfu.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://pgt.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bmx.vqdsnc.cn

[Q47] 与平均值比较
来源：http://dck.svipenyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rsx.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://xws.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nxk.zhaomingkeji.xyz

SELECT * FROM t WHERE c > 5;
来源：http://wmv.cashguo.top

[Q49] 更新单行
来源：http://dpm.nanxinkj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hrn.aizwys.cn

[Q50] 批量更新
来源：http://xca.aizwys.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ubl.meibo888.top

[Q51] 用子查询更新
来源：http://ccn.wangshuangyany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://aoh.chenzaomai.com

[Q52] 删除指定行
来源：http://hlh.meibo888.top

DELETE FROM users WHERE id = 10;
来源：http://cck.sysykeji.top

[Q53] 按条件删除
来源：http://woa.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dfo.uphjek.com

[Q54] 清空表
来源：http://kya.redwolf501.top

TRUNCATE TABLE logs;
来源：http://can.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://bgr.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ldt.ydjk.org.cn

[Q56] 密集排名（并列不占位）
来源：http://ltw.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yfj.cdnleiting.top

[Q57] 行号
来源：http://jpi.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nht.fehbvm.com

[Q58] 累计求和
来源：http://zfc.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://tbc.yanxiufei.cn

[Q59] 分组内累计
来源：http://eyl.andypj.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wyd.wangshuangyany.cn

[Q60] 取上一行 / 下一行
来源：http://cgx.jiagoushi.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dgi.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://utt.zhongyouzk.top

[Q61] 移动平均
来源：http://olz.zhongyouzk.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qjv.tian-w.cn

[Q62] 分组占比
来源：http://rdv.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gkv.hcnkem.com

[Q63] 开启事务
来源：http://poa.zhongyouzk.top

START TRANSACTION;                -- 或 BEGIN
来源：http://bfa.jiagoushi.top

[Q64] 提交事务
来源：http://tob.yonumen.top

COMMIT;
来源：http://ohk.hnxiangtu.top

[Q65] 回滚事务
来源：http://ymg.sufxvd.cn

ROLLBACK;
来源：http://djh.guannengcc.top

[Q66] 行锁查询
来源：http://hzq.jianghu66.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vbs.yj20258888.top

[Q67] 设置隔离级别
来源：http://jpd.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mmo.epnwcf.com

[Q68] 保存点
来源：http://hri.chenlongwang.top

SAVEPOINT sp1;
来源：http://nyc.tianlin.xyz

ROLLBACK TO sp1;
来源：http://wie.nanxinkj.top

[Q69] 查看执行计划
来源：http://rtd.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wku.9152youxi.cn

[Q70] 更新统计信息
来源：http://fug.ydzc1.top

ANALYZE TABLE users;
来源：http://ivh.shanyushiyangkeji.top

[Q71] 查看建表语句
来源：http://mvf.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://twr.nanxinkj.top

[Q72] 查看索引
来源：http://kjq.zhoulong.xyz

SHOW INDEX FROM users;
来源：http://nxr.kuanghao11.cn

[Q73] 查看表状态
来源：http://lrq.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://smb.0kj1m.cn

[Q74] 强制使用索引
来源：http://qtz.aibaodan.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qti.feifeiyinyue.top

[Q75] 日期格式化
来源：http://xzu.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vax.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bwi.sufxvd.cn

[Q76] 按天统计
来源：http://myp.guannengcc.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ttx.yuanzhike.top

[Q77] 时间加减
来源：http://zfr.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ogs.nanxinkj.top

[Q78] 当前时间
来源：http://thr.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qvt.xuanzx.com

[Q79] 字符串拼接
来源：http://dqe.cdnleiting.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yyn.jinqigufen.top

[Q80] 字符串截取
来源：http://vus.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://grn.wangdashe.top

[Q81] 字符串替换
来源：http://ctd.svipenyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qeg.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://pmo.yonumen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qkl.hongshengwenyu.top

[Q83] 大小写转换
来源：http://jrz.zycfv.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nox.xinyue.icu

[Q84] 去除首尾空格
来源：http://yvr.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://wgr.zdbjq.cn

[Q85] 数值取整
来源：http://phz.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eto.xingfuxueyuan.xyz

[Q86] 读取 JSON 字段
来源：http://eed.zhongyouzk.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jeh.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://eqb.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pdn.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://gld.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://akn.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mwy.bbcook.cn

[Q89] 判断表是否存在
来源：http://jgu.daria6918.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kmf.ppjwa.cn

[Q90] 生成序号列
来源：http://glg.9152youxi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pzi.dianchejie.cn

================================================================================
来源：http://iup.hywenlv.cn

R. Bash 专题
来源：http://iah.gotoacloud.top

================================================================================
来源：http://ahb.jinqigufen.top

[R01] shebang 与严格模式
来源：http://nja.gogol.net.cn

#!/usr/bin/env bash
来源：http://yip.gzhubu.top

set -euo pipefail
来源：http://xwx.daria6918.cn

[R02] 变量赋值与使用
来源：http://vac.sweek.top

name="Tom"; echo "$name"
来源：http://jzb.xziqi.cn

[R03] 只读变量
来源：http://qok.gzhubu.top

readonly PI=3.14
来源：http://ubs.fengsongda.top

[R04] 位置参数
来源：http://kvb.cashguo.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fdk.redwolf501.top

[R05] 参数默认值
来源：http://ece.meibo888.top

name="${1:-default}"
来源：http://wwu.xuanzx.com

[R06] 判断命令是否存在
来源：http://tli.daxiang520.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rxa.chenlongwang.top

[R07] if 判断文件
来源：http://hoc.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lkk.yanxiufei.cn

[R08] 数值比较
来源：http://fjv.sxryk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uck.guannengcc.top

[R09] 字符串比较
来源：http://cym.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ejc.gotoacloud.top

[R10] 正则匹配
来源：http://ntk.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gby.nanxuanxn.top

[R11] case 多分支
来源：http://hrp.shanyushiyangtech.top

case "$1" in
来源：http://hdg.yj20258888.top

start) echo "启动" ;;
来源：http://ttw.uphjek.com

stop)  echo "停止" ;;
来源：http://vox.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://vbe.52xcode.cn

esac
来源：http://ryv.yongpay.top

[R12] for 遍历文件
来源：http://tgz.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://jfz.xuanzx.com

[R13] for 计数循环
来源：http://mdn.yonumen.top

for i in {1..10}; do echo "$i"; done
来源：http://kae.yongpay.top

[R14] C 风格 for
来源：http://jff.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rxo.jinqigfzy.top

[R15] while 逐行读文件
来源：http://rqq.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pgy.tanke756.top

[R16] until 等待条件
来源：http://wjt.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xth.gaohongyu789.top

[R17] 数组定义与取值
来源：http://mvg.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://rpr.yueranfly.top

[R18] 遍历数组
来源：http://rjr.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jpp.yj20258888.top

[R19] 数组长度
来源：http://ggf.zhaomingkeji.xyz

echo "${#arr[@]}"
来源：http://fdo.xinyue.icu

[R20] 关联数组（字典）
来源：http://obc.vehdjk.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://epr.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://xdg.shanyushiyangtech.top

echo "${#s}"
来源：http://uwl.hnxiangtu.top

[R22] 截取子串
来源：http://tog.hesvh.cn

echo "${s:0:5}"
来源：http://eah.gzhubu.top

[R23] 字符串替换
来源：http://nig.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gzb.gotoacloud.top

[R24] 大小写转换
来源：http://dsv.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qfu.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://loi.havefunace.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dmm.wangdashe.top

[R26] 命令替换
来源：http://ibr.yj20258.top

now=$(date +%F); echo "$now"
来源：http://mqx.jqgufenzy.top

[R27] 算术展开
来源：http://avw.yvedp.cn

echo $((1 + 2 * 3))
来源：http://anx.hysaishi.cn

[R28] 浮点运算
来源：http://zcz.mhx1999.top

echo "scale=2; 10/3" | bc
来源：http://vlu.shanyushiyangtech.top

[R29] 定义函数
来源：http://upz.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yoe.jlsjyb.cn

[R30] 函数返回状态码
来源：http://gxh.jlsjyb.cn

f() { return 0; }; f || echo "失败了"
来源：http://uri.dianchejie.cn

[R31] 局部变量
来源：http://jvg.quarkkingdee.top

f() { local x=1; echo "$x"; }
来源：http://lch.shangyingyoupin.top

[R32] 参数个数校验
来源：http://eom.havefunace.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bhr.ivvv.top

[R33] 捕获错误并提示行号
来源：http://abl.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mpi.cdnleiting.top

[R34] 退出时清理
来源：http://zbd.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://yni.aizwys.cn

[R35] 后台执行并等待
来源：http://mqi.meibo888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://day.sxryk.cn

[R36] 并发执行多个任务
来源：http://wpe.zdqjudy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ovo.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://eyp.9152youxi.cn

files=$(ls -1)
来源：http://aez.fktsv.cn

[R38] 管道串联
来源：http://cin.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://esw.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://dke.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://ygt.sufxvd.cn

[R40] 追加写日志
来源：http://hvr.tian-w.cn

echo "log" >> out.log
来源：http://uhg.svipenyu.cn

[R41] 丢弃输出
来源：http://jwe.316326.xyz

cmd >/dev/null 2>&1
来源：http://jhq.cashguo.top

[R42] 输入重定向
来源：http://clc.jinghuilouyu.cn

wc -l < a.txt
来源：http://lwf.shanyushiyangtech.top

[R43] 按名字查找文件
来源：http://xyu.jqgfzy.top

find . -name "*.log" -type f
来源：http://efz.sufxvd.cn

[R44] 按修改时间查找
来源：http://xua.pengpengdd.cyou

find . -mtime -7 -type f
来源：http://lym.aibaodan.cn

[R45] 批量删除
来源：http://vjj.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://jah.cheryme.top

[R46] 递归替换文件内容
来源：http://udr.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rte.yueranfly.top

[R47] sed 单行替换
来源：http://hhh.jqgfzy.top


<!-- 参考信息 -->