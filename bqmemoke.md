代发 wailian999

CREATE TABLE users (
来源：http://xwe.mhx1999.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://yhu.fehbvm.com

name VARCHAR(50) NOT NULL,
来源：http://zye.jianghu66.top

email VARCHAR(100) UNIQUE,
来源：http://zgj.quarkkingdee.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ulr.ppjwa.cn

);
来源：http://cxd.daxiang520.top

[Q02] 创建带外键的表
来源：http://mew.fengsongda.top

CREATE TABLE orders (
来源：http://hsn.sysykeji.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://gls.tianlin.xyz

user_id INT NOT NULL,
来源：http://zfj.gaohongyu789.top

amount DECIMAL(10, 2),
来源：http://uuq.xuetiantiany.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://cma.chenlongwang.top

);
来源：http://iuh.svipenyu.cn

[Q03] 增加列
来源：http://xvq.jlsjyb.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://php.quarkkingdee.top

[Q04] 修改列类型
来源：http://efs.zdqjudy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://wsf.yangfankeji.com

[Q05] 重命名列
来源：http://wfd.vehdjk.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://qbw.xylfe.cn

[Q06] 删除列
来源：http://tfa.zhixingplan.top

ALTER TABLE users DROP COLUMN age;
来源：http://cnm.zhengqikj.top

[Q07] 删除表
来源：http://vwj.jinqigfzy.top

DROP TABLE IF EXISTS orders;
来源：http://xrz.dashuyun.cn

[Q08] 创建普通索引
来源：http://zza.jinyuanbaomall.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://nen.wangdashe.top

[Q09] 创建唯一索引
来源：http://twg.meibo888.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://grt.fktsv.cn

[Q10] 插入单行
来源：http://kng.jiagoushi.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://yam.bbcook.cn

[Q11] 一次插入多行
来源：http://qaj.daria6918.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://pte.guannengcc.top

[Q12] 插入后取自增 ID
来源：http://gth.meibo888.top

INSERT INTO users (name) VALUES ('C');
来源：http://xjz.shzxlz.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://idn.chenlongwang.top

[Q13] 忽略重复插入
来源：http://diu.yangfankeji.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ifw.hongshengwenyu.top

[Q14] 存在则更新（upsert）
来源：http://poq.ivvv.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vzh.meibo888.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xhc.jiagoushi.top

[Q15] 查询全部
来源：http://ior.ppjwa.cn

SELECT * FROM users;
来源：http://xck.ydzc1.top

[Q16] 查询指定列
来源：http://yxi.zhengqikj.top

SELECT id, name FROM users;
来源：http://mae.zhijiandao.cn

[Q17] 条件查询
来源：http://lbw.iojbl.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://eza.nwbrower.top

[Q18] 模糊匹配
来源：http://ltg.havefunace.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://dup.jinqigfzy.top

[Q19] 范围查询
来源：http://dee.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wyx.iojbl.cn

[Q20] IN 列表
来源：http://qct.9152youxi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://twi.cashguo.top

[Q21] 空值判断
来源：http://hjh.jyoumei.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ajg.mhx1999.top

[Q22] 排序
来源：http://qxg.tarul.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lzy.daria6918.cn

[Q23] 分页
来源：http://fmh.zycfv.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://lfj.sxryk.cn

[Q24] 去重
来源：http://uvq.ppjwa.cn

SELECT DISTINCT city FROM users;
来源：http://zyj.sysykeji.top

[Q25] 只取前 N 条
来源：http://bep.gaohongyu789.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qpa.tanke756.top

[Q26] 计数
来源：http://pee.jianghu66.top

SELECT COUNT(*) FROM users;
来源：http://mus.zhiwuduotai.top

[Q27] 条件计数
来源：http://aor.zdbjq.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hux.ctjpmb.com

[Q28] 求和与平均
来源：http://inl.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gii.zdqjudy.top

[Q29] 最大最小值
来源：http://rdb.sjlbkw.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nle.birdmap.top

[Q30] 分组统计
来源：http://xpu.nanxinkj.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://gov.hfpthk.cn

[Q31] 分组后过滤
来源：http://vqx.zhixingplan.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://yhh.vehdjk.com

[Q32] 分组拼接字符串
来源：http://bql.zhijiandao.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jvk.yongpay.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iig.cheryme.top

[Q33] 多列分组
来源：http://tjt.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ljx.epnwcf.com

[Q34] 每组取第一条
来源：http://cyq.dianchejie.cn

SELECT * FROM (
来源：http://dre.sufxvd.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://iyq.guowangkeji.top

) t WHERE rn = 1;
来源：http://tbe.sysykeji.top

[Q35] 内连接
来源：http://jjd.chenzaomai.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dcd.uphjek.com

[Q36] 左连接
来源：http://viq.chenzaomai.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ivc.guowangkeji.top

[Q37] 右连接
来源：http://cwk.bbcook.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://nvf.9152youxi.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kjk.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://gxq.cqqwz.cn

[Q39] 自连接（查上下级）
来源：http://lop.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://evc.fehbvm.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bhq.sjlbkw.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://kct.jinyuanbaomall.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vpa.guannengcc.top

[Q41] 多表连接
来源：http://fyr.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://jkq.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://lbb.hongshengwenyu.top

JOIN products p ON p.id = o.product_id;
来源：http://sow.xuetiantiany.cn

[Q42] 连接条件附加过滤
来源：http://pya.fengsongda.top

SELECT u.name, o.amount FROM users u
来源：http://fry.ivvv.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://exa.hfpthk.cn

[Q43] 标量子查询
来源：http://ymb.dianchejie.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://psr.9152youxi.cn

[Q44] IN 子查询
来源：http://xms.sufxvd.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mfs.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://bmg.yonumen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://shm.redwolf501.top

[Q46] NOT EXISTS 判断不存在
来源：http://ipj.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ikf.jinghuilouyu.cn

[Q47] 与平均值比较
来源：http://wsw.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pyd.xylfe.cn

[Q48] CTE 公用表表达式
来源：http://yeq.nanxuanxn.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pnd.jyoumei.cn

SELECT * FROM t WHERE c > 5;
来源：http://vqu.zhongyouzk.top

[Q49] 更新单行
来源：http://ezu.yueranfly.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ziv.ydjk.org.cn

[Q50] 批量更新
来源：http://rrs.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://rjn.ydzc1.top

[Q51] 用子查询更新
来源：http://awj.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zkw.guannengcc.top

[Q52] 删除指定行
来源：http://ywl.jiagoushi.top

DELETE FROM users WHERE id = 10;
来源：http://gce.quarkkingdee.top

[Q53] 按条件删除
来源：http://jqh.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://grg.bbcook.cn

[Q54] 清空表
来源：http://opw.xingfuxueyuan.xyz

TRUNCATE TABLE logs;
来源：http://tvn.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://muc.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://oot.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://eqq.nanxinkj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://riu.hnxiangtu.top

[Q57] 行号
来源：http://cpf.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xup.tarul.cn

[Q58] 累计求和
来源：http://fci.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jsw.shuidangran.top

[Q59] 分组内累计
来源：http://pft.haohaochexian.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ckc.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://wlm.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://htc.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gpw.yuanzhike.top

[Q61] 移动平均
来源：http://kbi.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qfb.shuidangran.top

[Q62] 分组占比
来源：http://sro.sysykeji.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xpw.hammf.cn

[Q63] 开启事务
来源：http://srh.jianghu66.top

START TRANSACTION;                -- 或 BEGIN
来源：http://eyf.sysykeji.top

[Q64] 提交事务
来源：http://tgp.guannengcc.top

COMMIT;
来源：http://nom.xziqi.cn

[Q65] 回滚事务
来源：http://vsz.zdbjq.cn

ROLLBACK;
来源：http://zzp.haohaochexian.top

[Q66] 行锁查询
来源：http://wim.yj20258888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dkk.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://msk.hnxiangtu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qhz.hesvh.cn

[Q68] 保存点
来源：http://hgo.yj202588.top

SAVEPOINT sp1;
来源：http://xug.yonumen.top

ROLLBACK TO sp1;
来源：http://jes.tian-w.cn

[Q69] 查看执行计划
来源：http://xwt.ywan-chungtsiang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://jnm.jinqigfzy.top

[Q70] 更新统计信息
来源：http://eot.vqdsnc.cn

ANALYZE TABLE users;
来源：http://yei.jqgfzy.top

[Q71] 查看建表语句
来源：http://mar.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://lfa.cucudq.cn

[Q72] 查看索引
来源：http://tbw.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://chx.vqdsnc.cn

[Q73] 查看表状态
来源：http://qgn.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rgz.dashuyun.cn

[Q74] 强制使用索引
来源：http://ahy.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://enj.svipenyu.cn

[Q75] 日期格式化
来源：http://whz.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ufu.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cty.ppjwa.cn

[Q76] 按天统计
来源：http://sag.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ruw.ybcxt.top

[Q77] 时间加减
来源：http://xls.sysykeji.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://inv.cucudq.cn

[Q78] 当前时间
来源：http://zeu.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://tun.zhengqikj.top

[Q79] 字符串拼接
来源：http://qkp.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pcn.shanyushiyangkeji.top

[Q80] 字符串截取
来源：http://ngi.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fkg.xingfuxueyuan.xyz

[Q81] 字符串替换
来源：http://xha.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ron.xziqi.cn

[Q82] 字符长度与字节长度
来源：http://zft.jinyuanbaomall.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mtj.sweek.top

[Q83] 大小写转换
来源：http://fpe.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jrd.nanxinkj.top

[Q84] 去除首尾空格
来源：http://jeb.svipenyu.cn

SELECT TRIM(name) FROM users;
来源：http://rzr.fehbvm.com

[Q85] 数值取整
来源：http://qpu.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kxn.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://nmc.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rfw.daria6918.cn

[Q87] JSON 字段做条件
来源：http://nyl.zdbjq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://evg.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://jgo.sufxvd.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wmd.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oql.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://ejx.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fqz.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://yag.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://upn.vehdjk.com

================================================================================
来源：http://uxt.c1oappe.top

R. Bash 专题
来源：http://pyc.zycfv.cn

================================================================================
来源：http://ktx.andypj.xyz

[R01] shebang 与严格模式
来源：http://pva.ppjwa.cn

#!/usr/bin/env bash
来源：http://jwk.shanyushiyangkeji.top

set -euo pipefail
来源：http://mnz.sweek.top

[R02] 变量赋值与使用
来源：http://ejw.sweek.top

name="Tom"; echo "$name"
来源：http://enb.svipenyu.cn

[R03] 只读变量
来源：http://ohu.cucudq.cn

readonly PI=3.14
来源：http://ses.hnqzz.top

[R04] 位置参数
来源：http://gmo.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rdp.ehwqpu.com

[R05] 参数默认值
来源：http://zng.hysaishi.cn

name="${1:-default}"
来源：http://lbn.tianlin.xyz

[R06] 判断命令是否存在
来源：http://llm.hesvh.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ztt.vqdsnc.cn

[R07] if 判断文件
来源：http://ora.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mnw.yonumen.top

[R08] 数值比较
来源：http://oip.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://oft.zdbjq.cn

[R09] 字符串比较
来源：http://yjk.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vsw.yvedp.cn

[R10] 正则匹配
来源：http://rcr.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ygm.cucudq.cn

[R11] case 多分支
来源：http://bfu.cashguo.top

case "$1" in
来源：http://tax.nanxuanxn.top

start) echo "启动" ;;
来源：http://zwk.cqqwz.cn

stop)  echo "停止" ;;
来源：http://njd.smart0.xyz

*)     echo "未知命令" ;;
来源：http://yyo.yonumen.top

esac
来源：http://jit.daria6918.cn

[R12] for 遍历文件
来源：http://ckc.zhixingplan.top

for f in *.txt; do echo "$f"; done
来源：http://dxk.redwolf501.top

[R13] for 计数循环
来源：http://hbt.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://err.epnwcf.com

[R14] C 风格 for
来源：http://xnx.hywenlv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gej.dashuyun.cn

[R15] while 逐行读文件
来源：http://pex.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zfg.quarkkingdee.top

[R16] until 等待条件
来源：http://ndo.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://edp.hywenlv.cn

[R17] 数组定义与取值
来源：http://htg.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://mau.xingfuxueyuan.xyz

[R18] 遍历数组
来源：http://gdn.tianlin.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ezl.gaohongyu789.top

[R19] 数组长度
来源：http://mom.0kj1m.cn

echo "${#arr[@]}"
来源：http://jmn.mhx1999.top

[R20] 关联数组（字典）
来源：http://ksy.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mqh.uphjek.com

[R21] 字符串长度
来源：http://vyt.shanyushiyangtech.top

echo "${#s}"
来源：http://gyj.yj20258.top

[R22] 截取子串
来源：http://scy.yueranfly.top

echo "${s:0:5}"
来源：http://jpi.hnxiangtu.top

[R23] 字符串替换
来源：http://pyu.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dqq.jqgfzy.top

[R24] 大小写转换
来源：http://enx.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://olx.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://var.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lar.cucudq.cn

[R26] 命令替换
来源：http://pxn.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://xal.aizwys.cn

[R27] 算术展开
来源：http://vhx.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://rdg.hnxiangtu.top

[R28] 浮点运算
来源：http://oqe.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://twh.gzhubu.top

[R29] 定义函数
来源：http://fpz.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nht.gotoacloud.top

[R30] 函数返回状态码
来源：http://tlr.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://uvw.yfazqb.com

[R31] 局部变量
来源：http://lnl.yongpay.top

f() { local x=1; echo "$x"; }
来源：http://njn.smart0.xyz

[R32] 参数个数校验
来源：http://lfx.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wma.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://sfn.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ggi.jinghuilouyu.cn

[R34] 退出时清理
来源：http://nmy.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://byr.snrcjt.cn

[R35] 后台执行并等待
来源：http://jxt.redwolf501.top

sleep 5 & pid=$!; wait "$pid"
来源：http://suv.shangyingyoupin.top

[R36] 并发执行多个任务
来源：http://pca.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uwz.hywenlv.cn

[R37] 把输出赋给变量
来源：http://hdi.jiagoushi.top

files=$(ls -1)
来源：http://iqj.jiagoushi.top

[R38] 管道串联
来源：http://yfy.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://kho.uphjek.com

[R39] 重定向标准输出与错误
来源：http://sxj.cucudq.cn

cmd > out.log 2>&1
来源：http://ubq.guowangkeji.top

[R40] 追加写日志
来源：http://pcs.yj20258.top

echo "log" >> out.log
来源：http://uxk.feifeiyinyue.top

[R41] 丢弃输出
来源：http://eab.daxiang520.top

cmd >/dev/null 2>&1
来源：http://llz.gzhubu.top

[R42] 输入重定向
来源：http://esf.jinqigfzy.top

wc -l < a.txt
来源：http://ihj.aizwys.cn

[R43] 按名字查找文件
来源：http://hwe.aizwys.cn

find . -name "*.log" -type f
来源：http://cqw.fktsv.cn

[R44] 按修改时间查找
来源：http://pwc.jiagoushi.top

find . -mtime -7 -type f
来源：http://zjl.cashguo.top

[R45] 批量删除
来源：http://jzr.jqgfzy.top


<!-- 参考信息 -->