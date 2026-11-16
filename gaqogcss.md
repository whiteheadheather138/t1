代发 wailian999

CREATE TABLE users (
来源：http://wiy.ywan-chungtsiang.top

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://hjg.jinghuilouyu.cn

name VARCHAR(50) NOT NULL,
来源：http://xur.wangdashe.top

email VARCHAR(100) UNIQUE,
来源：http://aeu.mhx1999.top

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://fzp.jqgufenzy.top

);
来源：http://mnv.0kj1m.cn

[Q02] 创建带外键的表
来源：http://pvi.svipenyu.cn

CREATE TABLE orders (
来源：http://obj.ppjwa.cn

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://sgj.jinyuanbaomall.cn

user_id INT NOT NULL,
来源：http://zzd.zhaomingkeji.xyz

amount DECIMAL(10, 2),
来源：http://tyq.andypj.xyz

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://uhf.0kj1m.cn

);
来源：http://qxf.hammf.cn

[Q03] 增加列
来源：http://ltq.shanyushiyangkeji.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://lmx.meibo888.top

[Q04] 修改列类型
来源：http://tbp.yonumen.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xxx.sufxvd.cn

[Q05] 重命名列
来源：http://rxn.smart0.xyz

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://hab.vehdjk.com

[Q06] 删除列
来源：http://ajl.iojbl.cn

ALTER TABLE users DROP COLUMN age;
来源：http://ryv.havefunace.top

[Q07] 删除表
来源：http://yhz.zycfv.cn

DROP TABLE IF EXISTS orders;
来源：http://uhr.yanxiufei.cn

[Q08] 创建普通索引
来源：http://ivc.zycfv.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://kim.ydzc1.top

[Q09] 创建唯一索引
来源：http://kmc.xuanzx.com

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pgy.pengpengdd.cyou

[Q10] 插入单行
来源：http://tmn.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://pud.jianghu66.top

[Q11] 一次插入多行
来源：http://qty.andypj.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://owl.xuetiantiany.cn

[Q12] 插入后取自增 ID
来源：http://xai.cucudq.cn

INSERT INTO users (name) VALUES ('C');
来源：http://fpb.tianlin.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wck.fanxiaobao.xyz

[Q13] 忽略重复插入
来源：http://jzu.jinyuanbaomall.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://oms.dashuyun.cn

[Q14] 存在则更新（upsert）
来源：http://gqt.mhx1999.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://dhe.vehdjk.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://ftn.snrcjt.cn

[Q15] 查询全部
来源：http://vlk.yfazqb.com

SELECT * FROM users;
来源：http://esw.jinyuanbaomall.cn

[Q16] 查询指定列
来源：http://ier.birdmap.top

SELECT id, name FROM users;
来源：http://rdm.jlsjyb.cn

[Q17] 条件查询
来源：http://jzr.ctjpmb.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://pds.redwolf501.top

[Q18] 模糊匹配
来源：http://vyk.jqgfzy.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wny.ppjwa.cn

[Q19] 范围查询
来源：http://erk.svipenyu.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://vpd.fktsv.cn

[Q20] IN 列表
来源：http://zpf.yongpay.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://gid.cheryme.top

[Q21] 空值判断
来源：http://imm.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://guz.dashuyun.cn

[Q22] 排序
来源：http://tmt.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zua.smart0.xyz

[Q23] 分页
来源：http://pxn.pengpengdd.cyou

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://rgp.xuetiantiany.cn

[Q24] 去重
来源：http://ase.sysykeji.top

SELECT DISTINCT city FROM users;
来源：http://igy.xylfe.cn

[Q25] 只取前 N 条
来源：http://otm.zhoulong.xyz

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://rte.hysaishi.cn

[Q26] 计数
来源：http://kyx.jinqigufen.top

SELECT COUNT(*) FROM users;
来源：http://dqf.aizwys.cn

[Q27] 条件计数
来源：http://smg.yj20258888.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vgh.sjlbkw.cn

[Q28] 求和与平均
来源：http://xan.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pet.mhx1999.top

[Q29] 最大最小值
来源：http://ahx.smart0.xyz

SELECT MAX(age), MIN(age) FROM users;
来源：http://irr.vqdsnc.cn

[Q30] 分组统计
来源：http://awf.yuxming.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dlr.pycfn.com

[Q31] 分组后过滤
来源：http://vud.yvedp.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://llj.yongpay.top

[Q32] 分组拼接字符串
来源：http://dpv.pengpengdd.cyou

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://iuo.feifeiyinyue.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://gpr.cdnleiting.top

[Q33] 多列分组
来源：http://ryq.fktsv.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://vyr.ppjwa.cn

[Q34] 每组取第一条
来源：http://gnk.hesvh.cn

SELECT * FROM (
来源：http://vcf.jinyuanbaomall.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vhq.fengsongda.top

) t WHERE rn = 1;
来源：http://usb.sysykeji.top

[Q35] 内连接
来源：http://jth.andypj.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://gld.zhengqikj.top

[Q36] 左连接
来源：http://yve.daxiang520.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://nto.yuanzhike.top

[Q37] 右连接
来源：http://ljy.feifeiyinyue.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cjk.daxiang520.top

[Q38] 全外连接（PostgreSQL）
来源：http://tly.shzxlz.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ljl.yuanzhike.top

[Q39] 自连接（查上下级）
来源：http://pmj.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://coj.shzxlz.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ahj.zhijiandao.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fhi.jinqigufen.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vlr.tarul.cn

[Q41] 多表连接
来源：http://rgt.chenlongwang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://hcz.xylfe.cn

JOIN users u ON u.id = o.user_id
来源：http://whh.316326.xyz

JOIN products p ON p.id = o.product_id;
来源：http://bxa.nwbrower.top

[Q42] 连接条件附加过滤
来源：http://jmc.vqdsnc.cn

SELECT u.name, o.amount FROM users u
来源：http://gft.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://dyy.c1oappe.top

[Q43] 标量子查询
来源：http://yic.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://apm.shanyushiyangtech.top

[Q44] IN 子查询
来源：http://axl.chenjidiqi.icu

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zxa.iojbl.cn

[Q45] EXISTS 判断存在
来源：http://fsj.jqgufenzy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gsv.ppjwa.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vfg.sjlbkw.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://evg.guowangkeji.top

[Q47] 与平均值比较
来源：http://anb.wangshuangyany.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hfx.andypj.xyz

[Q48] CTE 公用表表达式
来源：http://dju.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mlv.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://vdi.cdnleiting.top

[Q49] 更新单行
来源：http://eio.andypj.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://szc.52xcode.cn

[Q50] 批量更新
来源：http://yvi.cucudq.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yjn.yangfankeji.com

[Q51] 用子查询更新
来源：http://xlr.yfazqb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cye.yj20258.top

[Q52] 删除指定行
来源：http://sqm.shangyingyoupin.top

DELETE FROM users WHERE id = 10;
来源：http://jzz.xylfe.cn

[Q53] 按条件删除
来源：http://mif.ydzc1.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://trs.ppjwa.cn

[Q54] 清空表
来源：http://fin.yonumen.top

TRUNCATE TABLE logs;
来源：http://vht.jinghuilouyu.cn

[Q55] 排名（并列占位）
来源：http://xbw.guowangkeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dsb.hesvh.cn

[Q56] 密集排名（并列不占位）
来源：http://czc.ppjwa.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kaw.daxiang520.top

[Q57] 行号
来源：http://abt.yueranfly.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cbw.bbcook.cn

[Q58] 累计求和
来源：http://lxk.pengpengdd.cyou

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jem.fengsongda.top

[Q59] 分组内累计
来源：http://cjp.xylfe.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jdd.mhx1999.top

[Q60] 取上一行 / 下一行
来源：http://wje.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ncx.jqgfzy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ldx.hnxiangtu.top

[Q61] 移动平均
来源：http://qza.sxryk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gxm.yueranfly.top

[Q62] 分组占比
来源：http://lbc.tian-w.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wht.meibo888.top

[Q63] 开启事务
来源：http://rdd.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kjg.jqgufenzy.top

[Q64] 提交事务
来源：http://yvv.havefunace.top

COMMIT;
来源：http://qvc.snrcjt.cn

[Q65] 回滚事务
来源：http://tpu.zhongyouzk.top

ROLLBACK;
来源：http://vja.316326.xyz

[Q66] 行锁查询
来源：http://gnx.hcnkem.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wyc.zdqjudy.top

[Q67] 设置隔离级别
来源：http://ank.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ana.chenzaomai.com

[Q68] 保存点
来源：http://gem.316326.xyz

SAVEPOINT sp1;
来源：http://whw.meibo888.top

ROLLBACK TO sp1;
来源：http://fwe.svipenyu.cn

[Q69] 查看执行计划
来源：http://wkd.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ufi.fktsv.cn

[Q70] 更新统计信息
来源：http://fhk.yuxming.cn

ANALYZE TABLE users;
来源：http://xkp.zhijiandao.cn

[Q71] 查看建表语句
来源：http://ckl.ydzc1.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ddg.yj20258888.top

[Q72] 查看索引
来源：http://kwg.cashguo.top

SHOW INDEX FROM users;
来源：http://trm.chenjidiqi.icu

[Q73] 查看表状态
来源：http://qqm.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://wcf.jqgufenzy.top

[Q74] 强制使用索引
来源：http://jku.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://huu.cucudq.cn

[Q75] 日期格式化
来源：http://hwy.gotoacloud.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ewe.ppjwa.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://afl.c1oappe.top

[Q76] 按天统计
来源：http://jaj.kuanghao11.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kua.fengsongda.top

[Q77] 时间加减
来源：http://hle.meibo888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://opu.zhoulong.xyz

[Q78] 当前时间
来源：http://zsv.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://reb.yuxming.cn

[Q79] 字符串拼接
来源：http://okt.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bep.jqgufenzy.top

[Q80] 字符串截取
来源：http://qsg.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uua.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://rdy.guowangkeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vru.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://lqj.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ptf.bbcook.cn

[Q83] 大小写转换
来源：http://ynn.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lgj.havefunace.top

[Q84] 去除首尾空格
来源：http://sef.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://mzk.vehdjk.com

[Q85] 数值取整
来源：http://pqm.cashguo.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nxs.ppjwa.cn

[Q86] 读取 JSON 字段
来源：http://pmt.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dtf.zdbjq.cn

[Q87] JSON 字段做条件
来源：http://arw.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kqj.bbcook.cn

[Q88] 行转列（条件聚合）
来源：http://gdk.mhx1999.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cbw.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oqo.jlsjyb.cn

[Q89] 判断表是否存在
来源：http://cnh.9152youxi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://grg.tian-w.cn

[Q90] 生成序号列
来源：http://swe.0kj1m.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rtz.fanxiaobao.xyz

================================================================================
来源：http://tsa.pengpengdd.cyou

R. Bash 专题
来源：http://xzk.yonumen.top

================================================================================
来源：http://wjj.epnwcf.com

[R01] shebang 与严格模式
来源：http://mec.jiagoushi.top

#!/usr/bin/env bash
来源：http://eav.iojbl.cn

set -euo pipefail
来源：http://aep.ydzc1.top

[R02] 变量赋值与使用
来源：http://irt.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://yyz.zhiwuduotai.top

[R03] 只读变量
来源：http://xlg.xziqi.cn

readonly PI=3.14
来源：http://npz.pengpengdd.cyou

[R04] 位置参数
来源：http://azg.dashuyun.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bbn.ivvv.top

[R05] 参数默认值
来源：http://ixy.vqdsnc.cn

name="${1:-default}"
来源：http://fcm.dianchejie.cn

[R06] 判断命令是否存在
来源：http://nnm.cashguo.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lny.fktsv.cn

[R07] if 判断文件
来源：http://phw.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zsd.xinyue.icu

[R08] 数值比较
来源：http://enz.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hmc.zdqjudy.top

[R09] 字符串比较
来源：http://rta.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kji.fktsv.cn

[R10] 正则匹配
来源：http://xnw.jqgufenzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://suj.chenlongwang.top

[R11] case 多分支
来源：http://ozf.guannengcc.top

case "$1" in
来源：http://ami.zhongyouzk.top

start) echo "启动" ;;
来源：http://jkt.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://lqx.316326.xyz

*)     echo "未知命令" ;;
来源：http://ujn.aizwys.cn

esac
来源：http://vyr.sjlbkw.cn

[R12] for 遍历文件
来源：http://mrp.bjfxy.top

for f in *.txt; do echo "$f"; done
来源：http://gsv.9152youxi.cn

[R13] for 计数循环
来源：http://mmz.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://uvw.hfpthk.cn

[R14] C 风格 for
来源：http://hxc.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gev.vqdsnc.cn

[R15] while 逐行读文件
来源：http://til.zhiwuduotai.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gcm.mhx1999.top

[R16] until 等待条件
来源：http://skx.chenzaomai.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hnb.yj202588.top

[R17] 数组定义与取值
来源：http://bva.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ahk.ppjwa.cn

[R18] 遍历数组
来源：http://yxv.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dbr.mhx1999.top

[R19] 数组长度
来源：http://xwi.quarkkingdee.top

echo "${#arr[@]}"
来源：http://yxa.tanke756.top

[R20] 关联数组（字典）
来源：http://xwe.jqgfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lem.jinghuilouyu.cn

[R21] 字符串长度
来源：http://cxy.svipenyu.cn

echo "${#s}"
来源：http://xpn.havefunace.top

[R22] 截取子串
来源：http://kiq.52xcode.cn

echo "${s:0:5}"
来源：http://aks.tarul.cn

[R23] 字符串替换
来源：http://bvi.zycfv.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ljb.ivvv.top

[R24] 大小写转换
来源：http://afo.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://nfa.fanxiaobao.xyz

[R25] 去后缀 / 去前缀
来源：http://nsv.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rst.bjfxy.top

[R26] 命令替换
来源：http://ycq.yongpay.top

now=$(date +%F); echo "$now"
来源：http://tbp.jyoumei.cn

[R27] 算术展开
来源：http://rbo.bbcook.cn

echo $((1 + 2 * 3))
来源：http://bkc.jinqigfzy.top

[R28] 浮点运算
来源：http://bod.wangdashe.top

echo "scale=2; 10/3" | bc
来源：http://vak.gotoacloud.top

[R29] 定义函数
来源：http://hmp.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fdq.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://iwd.guannengcc.top

f() { return 0; }; f || echo "失败了"
来源：http://klc.chenjidiqi.icu

[R31] 局部变量
来源：http://ogv.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://sxa.nanxuanxn.top

[R32] 参数个数校验
来源：http://lan.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nrd.316326.xyz

[R33] 捕获错误并提示行号
来源：http://geu.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qzb.havefunace.top

[R34] 退出时清理
来源：http://epe.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xew.cashguo.top

[R35] 后台执行并等待
来源：http://jsi.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lsw.316326.xyz

[R36] 并发执行多个任务
来源：http://lni.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ktx.jinqigfzy.top

[R37] 把输出赋给变量
来源：http://wny.vehdjk.com

files=$(ls -1)
来源：http://wxj.smart0.xyz

[R38] 管道串联
来源：http://shv.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://ifu.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://hnp.ydjk.org.cn

cmd > out.log 2>&1
来源：http://msy.guowangkeji.top

[R40] 追加写日志
来源：http://yvf.xinyue.icu

echo "log" >> out.log
来源：http://fal.fktsv.cn

[R41] 丢弃输出
来源：http://axl.52xcode.cn

cmd >/dev/null 2>&1
来源：http://bag.xuanzx.com

[R42] 输入重定向
来源：http://zzn.haohaochexian.top

wc -l < a.txt
来源：http://mea.wangshuangyany.cn

[R43] 按名字查找文件
来源：http://mum.aibaodan.cn

find . -name "*.log" -type f
来源：http://olt.quarkkingdee.top

[R44] 按修改时间查找
来源：http://gxk.ybcxt.top

find . -mtime -7 -type f
来源：http://vnk.zhengqikj.top

[R45] 批量删除
来源：http://gef.shzxlz.cn


<!-- 参考信息 -->