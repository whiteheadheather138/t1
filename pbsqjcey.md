代发 wailian999

CREATE TABLE users (
来源：http://zgs.316326.xyz

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://quj.zycfv.cn

name VARCHAR(50) NOT NULL,
来源：http://frm.ybcxt.top

email VARCHAR(100) UNIQUE,
来源：http://pup.c1oappe.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://icd.fanxiaobao.xyz

);
来源：http://kbi.nanxuanxn.top

[Q02] 创建带外键的表
来源：http://qha.chenjidiqi.icu

CREATE TABLE orders (
来源：http://spf.yj20258888.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://vgq.ehwqpu.com

user_id INT NOT NULL,
来源：http://oiw.zhengqikj.top

amount DECIMAL(10, 2),
来源：http://dzw.ehwqpu.com

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ekk.fanxiaobao.xyz

);
来源：http://vjg.hysaishi.cn

[Q03] 增加列
来源：http://qha.shanyushiyangtech.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hbz.guowangkeji.top

[Q04] 修改列类型
来源：http://xyx.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://dcz.hnxiangtu.top

[Q05] 重命名列
来源：http://kfp.hesvh.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://fua.hfpthk.cn

[Q06] 删除列
来源：http://nzt.jianghu66.top

ALTER TABLE users DROP COLUMN age;
来源：http://rxm.nanxinkj.top

[Q07] 删除表
来源：http://owh.fzhhl.top

DROP TABLE IF EXISTS orders;
来源：http://fdd.gogol.net.cn

[Q08] 创建普通索引
来源：http://iii.shangyingyoupin.top

CREATE INDEX idx_users_email ON users(email);
来源：http://eog.iojbl.cn

[Q09] 创建唯一索引
来源：http://zny.sweek.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://bpp.chenzaomai.com

[Q10] 插入单行
来源：http://iww.ehwqpu.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ftt.uphjek.com

[Q11] 一次插入多行
来源：http://aph.havefunace.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gtb.yuxming.cn

[Q12] 插入后取自增 ID
来源：http://jsp.daxiang520.top

INSERT INTO users (name) VALUES ('C');
来源：http://xvh.haohaochexian.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://idk.xinyue.icu

[Q13] 忽略重复插入
来源：http://kpj.ybcxt.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oyd.cdnleiting.top

[Q14] 存在则更新（upsert）
来源：http://pxe.zhixingplan.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://als.fanxiaobao.xyz

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wlf.yanxiufei.cn

[Q15] 查询全部
来源：http://tkc.hammf.cn

SELECT * FROM users;
来源：http://qsa.nanxuanxn.top

[Q16] 查询指定列
来源：http://kpz.xinyue.icu

SELECT id, name FROM users;
来源：http://ivo.bjfxy.top

[Q17] 条件查询
来源：http://rqj.jlsjyb.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://san.cqqwz.cn

[Q18] 模糊匹配
来源：http://pxs.bbcook.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://rcm.yanxiufei.cn

[Q19] 范围查询
来源：http://qnm.yangfankeji.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vmp.chenzaomai.com

[Q20] IN 列表
来源：http://kev.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pyk.shanyushiyangkeji.top

[Q21] 空值判断
来源：http://yed.shuidangran.top

SELECT * FROM users WHERE email IS NULL;
来源：http://faf.nanxuanxn.top

[Q22] 排序
来源：http://xyt.ppjwa.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lly.jqgufenzy.top

[Q23] 分页
来源：http://sgt.zdbjq.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dlw.gaohongyu789.top

[Q24] 去重
来源：http://zak.cqqwz.cn

SELECT DISTINCT city FROM users;
来源：http://ebo.yanxiufei.cn

[Q25] 只取前 N 条
来源：http://myy.chenlongwang.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nis.tianlin.xyz

[Q26] 计数
来源：http://jxm.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://zkm.xziqi.cn

[Q27] 条件计数
来源：http://ewa.zhoulong.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nlt.aibaodan.cn

[Q28] 求和与平均
来源：http://vgh.zhaomingkeji.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://tyw.jqgfzy.top

[Q29] 最大最小值
来源：http://pah.jinqigufen.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://uuh.dianchejie.cn

[Q30] 分组统计
来源：http://gno.jqgfzy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://csc.kuanghao11.cn

[Q31] 分组后过滤
来源：http://vyp.aibaodan.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xcs.xingfuxueyuan.xyz

[Q32] 分组拼接字符串
来源：http://zca.jinghuilouyu.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://gnd.vqdsnc.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://upu.gogol.net.cn

[Q33] 多列分组
来源：http://eua.zhaomingkeji.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ndv.wangdashe.top

[Q34] 每组取第一条
来源：http://iyx.shanyushiyangtech.top

SELECT * FROM (
来源：http://evv.snrcjt.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://day.xziqi.cn

) t WHERE rn = 1;
来源：http://zjf.ydjk.org.cn

[Q35] 内连接
来源：http://hun.zhixingplan.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ddi.gotoacloud.top

[Q36] 左连接
来源：http://gvu.xuanzx.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://lxp.zhengqikj.top

[Q37] 右连接
来源：http://ejq.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ish.zhengqikj.top

[Q38] 全外连接（PostgreSQL）
来源：http://bjy.jinqigfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dpb.mhx1999.top

[Q39] 自连接（查上下级）
来源：http://buy.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rxm.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jfg.ywan-chungtsiang.top

[Q40] 交叉连接（笛卡尔积）
来源：http://jfy.yongpay.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cai.havefunace.top

[Q41] 多表连接
来源：http://soi.hammf.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://pup.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://cea.guannengcc.top

JOIN products p ON p.id = o.product_id;
来源：http://znq.tanke756.top

[Q42] 连接条件附加过滤
来源：http://vve.ydzc1.top

SELECT u.name, o.amount FROM users u
来源：http://kfi.sweek.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dmn.feifeiyinyue.top

[Q43] 标量子查询
来源：http://gas.sxryk.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lre.zycfv.cn

[Q44] IN 子查询
来源：http://gqq.shuidangran.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://giv.ctjpmb.com

[Q45] EXISTS 判断存在
来源：http://eas.birdmap.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vfb.tanke756.top

[Q46] NOT EXISTS 判断不存在
来源：http://aft.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vjs.zhongyouzk.top

[Q47] 与平均值比较
来源：http://kvo.zhaomingkeji.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oso.gaohongyu789.top

[Q48] CTE 公用表表达式
来源：http://aty.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://uwm.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://szc.yuxming.cn

[Q49] 更新单行
来源：http://kdz.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vru.zhengqikj.top

[Q50] 批量更新
来源：http://cxo.ydjk.org.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pjn.xuanzx.com

[Q51] 用子查询更新
来源：http://zzz.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dvl.smart0.xyz

[Q52] 删除指定行
来源：http://lse.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://ljz.ivvv.top

[Q53] 按条件删除
来源：http://tpd.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ade.birdmap.top

[Q54] 清空表
来源：http://czw.guannengcc.top

TRUNCATE TABLE logs;
来源：http://zfx.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://duz.zhaomingkeji.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://iqt.hywenlv.cn

[Q56] 密集排名（并列不占位）
来源：http://kmm.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pun.mhx1999.top

[Q57] 行号
来源：http://jef.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tnc.cheryme.top

[Q58] 累计求和
来源：http://kgj.9152youxi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kef.guowangkeji.top

[Q59] 分组内累计
来源：http://ptb.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jze.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://oya.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jbe.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gik.hnxiangtu.top

[Q61] 移动平均
来源：http://pak.jlsjyb.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://csg.snrcjt.cn

[Q62] 分组占比
来源：http://svm.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kiu.gaohongyu789.top

[Q63] 开启事务
来源：http://kaf.9152youxi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://wdd.fzhhl.top

[Q64] 提交事务
来源：http://gba.shuidangran.top

COMMIT;
来源：http://rdt.sxryk.cn

[Q65] 回滚事务
来源：http://bre.sysykeji.top

ROLLBACK;
来源：http://awo.fzhhl.top

[Q66] 行锁查询
来源：http://cqh.bbcook.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pmy.sufxvd.cn

[Q67] 设置隔离级别
来源：http://tck.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cjt.hnxiangtu.top

[Q68] 保存点
来源：http://sfs.sjlbkw.cn

SAVEPOINT sp1;
来源：http://hxq.ctjpmb.com

ROLLBACK TO sp1;
来源：http://pqb.daria6918.cn

[Q69] 查看执行计划
来源：http://sqw.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ela.yfazqb.com

[Q70] 更新统计信息
来源：http://hzr.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://jqx.guowangkeji.top

[Q71] 查看建表语句
来源：http://oqm.pycfn.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jsm.0kj1m.cn

[Q72] 查看索引
来源：http://ttr.cucudq.cn

SHOW INDEX FROM users;
来源：http://rcv.yfazqb.com

[Q73] 查看表状态
来源：http://jyr.sysykeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://lrl.hcnkem.com

[Q74] 强制使用索引
来源：http://tjo.gotoacloud.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://psq.yueranfly.top

[Q75] 日期格式化
来源：http://tzo.vehdjk.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qri.zhijiandao.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://erm.tarul.cn

[Q76] 按天统计
来源：http://hwm.jiagoushi.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ozt.cqqwz.cn

[Q77] 时间加减
来源：http://pis.guowangkeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dht.daria6918.cn

[Q78] 当前时间
来源：http://qms.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kik.bbcook.cn

[Q79] 字符串拼接
来源：http://hhz.yonumen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xbz.sjlbkw.cn

[Q80] 字符串截取
来源：http://hhz.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jng.ydjk.org.cn

[Q81] 字符串替换
来源：http://rvp.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wqz.hcnkem.com

[Q82] 字符长度与字节长度
来源：http://jfy.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mzy.zhixingplan.top

[Q83] 大小写转换
来源：http://mbn.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qnp.ppjwa.cn

[Q84] 去除首尾空格
来源：http://tvy.ydjk.org.cn

SELECT TRIM(name) FROM users;
来源：http://rci.cdnleiting.top

[Q85] 数值取整
来源：http://rgs.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hin.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://rdz.ydzc1.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ocy.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://gwa.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://muf.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://qie.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sxl.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rlh.zdbjq.cn

[Q89] 判断表是否存在
来源：http://twe.yfazqb.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://afs.ydjk.org.cn

[Q90] 生成序号列
来源：http://wgc.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ccj.ctjpmb.com

================================================================================
来源：http://lct.nanxuanxn.top

R. Bash 专题
来源：http://ubj.ppjwa.cn

================================================================================
来源：http://cvi.fehbvm.com

[R01] shebang 与严格模式
来源：http://vye.ctjpmb.com

#!/usr/bin/env bash
来源：http://hdr.zhiwuduotai.top

set -euo pipefail
来源：http://pay.shanyushiyangtech.top

[R02] 变量赋值与使用
来源：http://ndr.xylfe.cn

name="Tom"; echo "$name"
来源：http://tha.jinyuanbaomall.cn

[R03] 只读变量
来源：http://qxm.nanxuanxn.top

readonly PI=3.14
来源：http://qac.cdnleiting.top

[R04] 位置参数
来源：http://nli.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://edw.epnwcf.com

[R05] 参数默认值
来源：http://aas.epnwcf.com

name="${1:-default}"
来源：http://mgs.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://jxz.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oal.chenzaomai.com

[R07] if 判断文件
来源：http://azb.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://flf.316326.xyz

[R08] 数值比较
来源：http://eqx.tianlin.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://rui.tianlin.xyz

[R09] 字符串比较
来源：http://soy.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sxv.cqqwz.cn

[R10] 正则匹配
来源：http://xvy.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mqy.yfazqb.com

[R11] case 多分支
来源：http://yph.birdmap.top

case "$1" in
来源：http://bjd.yonumen.top

start) echo "启动" ;;
来源：http://yxh.cdnleiting.top

stop)  echo "停止" ;;
来源：http://lym.havefunace.top

*)     echo "未知命令" ;;
来源：http://abk.gzhubu.top

esac
来源：http://aod.52xcode.cn

[R12] for 遍历文件
来源：http://pdi.fanxiaobao.xyz

for f in *.txt; do echo "$f"; done
来源：http://xop.shanyushiyangkeji.top

[R13] for 计数循环
来源：http://stk.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://eln.yonumen.top

[R14] C 风格 for
来源：http://oyo.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fbu.zhiwuduotai.top

[R15] while 逐行读文件
来源：http://fbl.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mox.ppjwa.cn

[R16] until 等待条件
来源：http://wbk.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://taq.tanke756.top

[R17] 数组定义与取值
来源：http://ifz.nanxinkj.top

arr=(a b c); echo "${arr[0]}"
来源：http://qvg.yangfankeji.com

[R18] 遍历数组
来源：http://qpi.dianchejie.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zbb.hesvh.cn

[R19] 数组长度
来源：http://wci.jinqigfzy.top

echo "${#arr[@]}"
来源：http://hom.aizwys.cn

[R20] 关联数组（字典）
来源：http://anr.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://arn.zhaomingkeji.xyz

[R21] 字符串长度
来源：http://avg.sxryk.cn

echo "${#s}"
来源：http://aab.c1oappe.top

[R22] 截取子串
来源：http://hxc.daria6918.cn

echo "${s:0:5}"
来源：http://org.hongshengwenyu.top

[R23] 字符串替换
来源：http://ngs.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pod.xuanzx.com

[R24] 大小写转换
来源：http://awe.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fqz.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://syn.ydzc1.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bon.pengpengdd.cyou

[R26] 命令替换
来源：http://zdn.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://gnu.shanyushiyangtech.top

[R27] 算术展开
来源：http://lds.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://wgm.tarul.cn

[R28] 浮点运算
来源：http://bdc.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://drh.pengpengdd.cyou

[R29] 定义函数
来源：http://lzs.hnqzz.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wlp.chenlongwang.top

[R30] 函数返回状态码
来源：http://nje.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://xoj.wangdashe.top

[R31] 局部变量
来源：http://wwj.shzxlz.cn

f() { local x=1; echo "$x"; }
来源：http://bgk.cqqwz.cn

[R32] 参数个数校验
来源：http://umz.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yjd.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://usm.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://led.yvedp.cn

[R34] 退出时清理
来源：http://vjt.yj20258888.top

trap 'rm -f "$tmp"' EXIT
来源：http://usv.jinqigfzy.top

[R35] 后台执行并等待
来源：http://ndc.wangshuangyany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hqh.zycfv.cn

[R36] 并发执行多个任务
来源：http://lcs.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ozb.jqgfzy.top

[R37] 把输出赋给变量
来源：http://ndl.tarul.cn

files=$(ls -1)
来源：http://qwn.chenlongwang.top

[R38] 管道串联
来源：http://grt.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://bud.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://ylp.birdmap.top

cmd > out.log 2>&1
来源：http://lft.zdqjudy.top

[R40] 追加写日志
来源：http://dyc.yuanzhike.top

echo "log" >> out.log
来源：http://egk.birdmap.top

[R41] 丢弃输出
来源：http://hau.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://imu.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://yfu.jinqigfzy.top

wc -l < a.txt
来源：http://hfw.nwbrower.top

[R43] 按名字查找文件
来源：http://wgm.ppjwa.cn

find . -name "*.log" -type f
来源：http://lvl.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://uek.jiagoushi.top

find . -mtime -7 -type f
来源：http://ifb.haohaochexian.top

[R45] 批量删除
来源：http://ihy.cheryme.top


<!-- 参考信息 -->