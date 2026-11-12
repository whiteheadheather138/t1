代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://leq.vqdsnc.cn

user_id INT NOT NULL,
来源：http://zhd.shanyushiyangkeji.top

amount DECIMAL(10, 2),
来源：http://bez.cdnleiting.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://ahi.hfpthk.cn

);
来源：http://jcb.sjlbkw.cn

[Q03] 增加列
来源：http://hxc.havefunace.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://jar.quarkkingdee.top

[Q04] 修改列类型
来源：http://xmv.chenjidiqi.icu

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://kqx.yj20258888.top

[Q05] 重命名列
来源：http://gis.yfazqb.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wnv.yvedp.cn

[Q06] 删除列
来源：http://uqa.sysykeji.top

ALTER TABLE users DROP COLUMN age;
来源：http://vnf.c1oappe.top

[Q07] 删除表
来源：http://cgw.vqdsnc.cn

DROP TABLE IF EXISTS orders;
来源：http://zjk.smart0.xyz

[Q08] 创建普通索引
来源：http://cgx.jyoumei.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://rcm.bjfxy.top

[Q09] 创建唯一索引
来源：http://vxs.sysykeji.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ypk.52xcode.cn

[Q10] 插入单行
来源：http://ucw.hesvh.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mcv.nanxinkj.top

[Q11] 一次插入多行
来源：http://did.tanke756.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://vxu.gzhubu.top

[Q12] 插入后取自增 ID
来源：http://jou.sufxvd.cn

INSERT INTO users (name) VALUES ('C');
来源：http://eec.hnxiangtu.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://zyp.zycfv.cn

[Q13] 忽略重复插入
来源：http://ioc.wangshuangyany.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://sfi.yonumen.top

[Q14] 存在则更新（upsert）
来源：http://shx.uphjek.com

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://rhe.xuetiantiany.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://peo.hcnkem.com

[Q15] 查询全部
来源：http://yfs.aibaodan.cn

SELECT * FROM users;
来源：http://fsf.gaohongyu789.top

[Q16] 查询指定列
来源：http://acj.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://ylp.52xcode.cn

[Q17] 条件查询
来源：http://njn.vehdjk.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nym.zhongyouzk.top

[Q18] 模糊匹配
来源：http://zeq.yvedp.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://yrr.dashuyun.cn

[Q19] 范围查询
来源：http://jea.chenlongwang.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sub.snrcjt.cn

[Q20] IN 列表
来源：http://nwt.shanyushiyangtech.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wwz.aibaodan.cn

[Q21] 空值判断
来源：http://ecf.yonumen.top

SELECT * FROM users WHERE email IS NULL;
来源：http://vva.tianlin.xyz

[Q22] 排序
来源：http://vcu.shanyushiyangkeji.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ocd.jqgfzy.top

[Q23] 分页
来源：http://hph.sxryk.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://oef.daria6918.cn

[Q24] 去重
来源：http://xwk.gzhubu.top

SELECT DISTINCT city FROM users;
来源：http://njt.zhongyouzk.top

[Q25] 只取前 N 条
来源：http://dvy.bjfxy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://zfn.fanxiaobao.xyz

[Q26] 计数
来源：http://nvg.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://kgg.ctjpmb.com

[Q27] 条件计数
来源：http://eos.xuetiantiany.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zzq.mhx1999.top

[Q28] 求和与平均
来源：http://oak.jlsjyb.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xkm.yj202588.top

[Q29] 最大最小值
来源：http://uyd.xuetiantiany.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://cml.redwolf501.top

[Q30] 分组统计
来源：http://dpx.cucudq.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dve.daxiang520.top

[Q31] 分组后过滤
来源：http://qkx.ybcxt.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://aty.yuanzhike.top

[Q32] 分组拼接字符串
来源：http://jry.zycfv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vpt.yj202588.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fll.fengsongda.top

[Q33] 多列分组
来源：http://fad.hcnkem.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wov.ehwqpu.com

[Q34] 每组取第一条
来源：http://ofk.hesvh.cn

SELECT * FROM (
来源：http://ttw.uphjek.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uin.fehbvm.com

) t WHERE rn = 1;
来源：http://gho.xziqi.cn

[Q35] 内连接
来源：http://utr.shanyushiyangtech.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://upi.zycfv.cn

[Q36] 左连接
来源：http://kka.redwolf501.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://eey.uphjek.com

[Q37] 右连接
来源：http://qul.zhengqikj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fnz.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://njy.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://edj.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://uog.cdnleiting.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://czy.andypj.xyz

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pft.sxryk.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://rvp.cqqwz.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://eum.nanxuanxn.top

[Q41] 多表连接
来源：http://pip.jinghuilouyu.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://exq.316326.xyz

JOIN users u ON u.id = o.user_id
来源：http://bgi.havefunace.top

JOIN products p ON p.id = o.product_id;
来源：http://uhh.andypj.xyz

[Q42] 连接条件附加过滤
来源：http://yov.redwolf501.top

SELECT u.name, o.amount FROM users u
来源：http://ebw.pycfn.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://avl.snrcjt.cn

[Q43] 标量子查询
来源：http://svw.zdqjudy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lhv.yongpay.top

[Q44] IN 子查询
来源：http://vwu.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qjf.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://uoj.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kjp.fanxiaobao.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://dys.feifeiyinyue.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ohu.feifeiyinyue.top

[Q47] 与平均值比较
来源：http://fjp.bjfxy.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://gqw.cheryme.top

[Q48] CTE 公用表表达式
来源：http://arv.shanyushiyangtech.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ecs.pycfn.com

SELECT * FROM t WHERE c > 5;
来源：http://nqq.jinghuilouyu.cn

[Q49] 更新单行
来源：http://fxp.fktsv.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ywz.hammf.cn

[Q50] 批量更新
来源：http://bzr.yj20258.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gcm.sysykeji.top

[Q51] 用子查询更新
来源：http://sbk.cashguo.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wkw.ppjwa.cn

[Q52] 删除指定行
来源：http://fat.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://pxe.yanxiufei.cn

[Q53] 按条件删除
来源：http://vaw.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ooc.cucudq.cn

[Q54] 清空表
来源：http://rvi.xziqi.cn

TRUNCATE TABLE logs;
来源：http://sdr.jianghu66.top

[Q55] 排名（并列占位）
来源：http://nws.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rdj.aizwys.cn

[Q56] 密集排名（并列不占位）
来源：http://gjs.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zyt.9152youxi.cn

[Q57] 行号
来源：http://lqn.jqgfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zqe.yongpay.top

[Q58] 累计求和
来源：http://wlt.fengsongda.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nvf.zhiwuduotai.top

[Q59] 分组内累计
来源：http://jxz.dianchejie.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iaj.andypj.xyz

[Q60] 取上一行 / 下一行
来源：http://elx.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ugu.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://apo.kuanghao11.cn

[Q61] 移动平均
来源：http://wcm.sjlbkw.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vac.hnqzz.top

[Q62] 分组占比
来源：http://jov.316326.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ude.tianlin.xyz

[Q63] 开启事务
来源：http://mfp.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://bpz.svipenyu.cn

[Q64] 提交事务
来源：http://qdq.cheryme.top

COMMIT;
来源：http://eei.yuxming.cn

[Q65] 回滚事务
来源：http://hgr.sufxvd.cn

ROLLBACK;
来源：http://ccl.yangfankeji.com

[Q66] 行锁查询
来源：http://pep.xinyue.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ufo.iojbl.cn

[Q67] 设置隔离级别
来源：http://qlb.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://duj.hywenlv.cn

[Q68] 保存点
来源：http://aya.tanke756.top

SAVEPOINT sp1;
来源：http://yuo.haohaochexian.top

ROLLBACK TO sp1;
来源：http://nwn.andypj.xyz

[Q69] 查看执行计划
来源：http://una.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rmb.zhongyouzk.top

[Q70] 更新统计信息
来源：http://mnx.svipenyu.cn

ANALYZE TABLE users;
来源：http://omz.9152youxi.cn

[Q71] 查看建表语句
来源：http://gid.hcnkem.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eep.yuxming.cn

[Q72] 查看索引
来源：http://end.yj20258.top

SHOW INDEX FROM users;
来源：http://wje.sxryk.cn

[Q73] 查看表状态
来源：http://zlr.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://xvv.fehbvm.com

[Q74] 强制使用索引
来源：http://jek.ydzc1.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://amh.yj20258.top

[Q75] 日期格式化
来源：http://fob.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kfw.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://gtq.yanxiufei.cn

[Q76] 按天统计
来源：http://nvd.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ugf.tarul.cn

[Q77] 时间加减
来源：http://kej.sufxvd.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://syg.jyoumei.cn

[Q78] 当前时间
来源：http://jod.guowangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://azg.zycfv.cn

[Q79] 字符串拼接
来源：http://sjk.xinyue.icu

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fyw.pycfn.com

[Q80] 字符串截取
来源：http://ctl.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yzn.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://rvx.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://muw.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://ojm.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fbo.zhixingplan.top

[Q83] 大小写转换
来源：http://tow.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lrq.svipenyu.cn

[Q84] 去除首尾空格
来源：http://uqg.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://xhj.fanxiaobao.xyz

[Q85] 数值取整
来源：http://mwv.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bqj.316326.xyz

[Q86] 读取 JSON 字段
来源：http://osj.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uon.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://mxp.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rpl.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://fop.guannengcc.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tgc.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fza.cashguo.top

[Q89] 判断表是否存在
来源：http://vyu.zhiwuduotai.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xai.sufxvd.cn

[Q90] 生成序号列
来源：http://mep.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dnp.yonumen.top

================================================================================
来源：http://gxb.yuxming.cn

R. Bash 专题
来源：http://ddh.sufxvd.cn

================================================================================
来源：http://wbm.0kj1m.cn

[R01] shebang 与严格模式
来源：http://poz.ctjpmb.com

#!/usr/bin/env bash
来源：http://loi.ydzc1.top

set -euo pipefail
来源：http://hvh.zhiwuduotai.top

[R02] 变量赋值与使用
来源：http://rmt.havefunace.top

name="Tom"; echo "$name"
来源：http://prg.xziqi.cn

[R03] 只读变量
来源：http://gqw.fanxiaobao.xyz

readonly PI=3.14
来源：http://lnn.hammf.cn

[R04] 位置参数
来源：http://msf.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hze.zhixingplan.top

[R05] 参数默认值
来源：http://sti.chenlongwang.top

name="${1:-default}"
来源：http://jro.feifeiyinyue.top

[R06] 判断命令是否存在
来源：http://lnw.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://adf.daria6918.cn

[R07] if 判断文件
来源：http://olf.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rxe.hywenlv.cn

[R08] 数值比较
来源：http://lrn.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://prd.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://qgo.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cwg.ctjpmb.com

[R10] 正则匹配
来源：http://aag.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://aii.birdmap.top

[R11] case 多分支
来源：http://eev.vehdjk.com

case "$1" in
来源：http://oby.jinqigufen.top

start) echo "启动" ;;
来源：http://grn.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://isk.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://unw.kuanghao11.cn

esac
来源：http://mvp.mhx1999.top

[R12] for 遍历文件
来源：http://gqu.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://amk.tarul.cn

[R13] for 计数循环
来源：http://qxv.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://xjz.tanke756.top

[R14] C 风格 for
来源：http://ocv.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://llh.zycfv.cn

[R15] while 逐行读文件
来源：http://hmt.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vyb.bbcook.cn

[R16] until 等待条件
来源：http://osa.cqqwz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tua.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://dup.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://bkz.sweek.top

[R18] 遍历数组
来源：http://nmg.ywan-chungtsiang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uhr.kuanghao11.cn

[R19] 数组长度
来源：http://lwp.yangfankeji.com

echo "${#arr[@]}"
来源：http://qeg.fktsv.cn

[R20] 关联数组（字典）
来源：http://wxa.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rgz.jinqigfzy.top

[R21] 字符串长度
来源：http://vkx.zdbjq.cn

echo "${#s}"
来源：http://udn.yj20258.top

[R22] 截取子串
来源：http://lpu.jqgfzy.top

echo "${s:0:5}"
来源：http://qsu.meibo888.top

[R23] 字符串替换
来源：http://pot.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gno.zhongyouzk.top

[R24] 大小写转换
来源：http://iaw.smart0.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://pjj.cqqwz.cn

[R25] 去后缀 / 去前缀
来源：http://zat.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rcw.andypj.xyz

[R26] 命令替换
来源：http://ybk.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://zyu.yanxiufei.cn

[R27] 算术展开
来源：http://ioe.tian-w.cn

echo $((1 + 2 * 3))
来源：http://uvj.havefunace.top

[R28] 浮点运算
来源：http://xdx.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://cbg.yuxming.cn

[R29] 定义函数
来源：http://apt.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zpf.daria6918.cn

[R30] 函数返回状态码
来源：http://omv.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://uul.sweek.top

[R31] 局部变量
来源：http://qeu.c1oappe.top

f() { local x=1; echo "$x"; }
来源：http://qzf.epnwcf.com

[R32] 参数个数校验
来源：http://syq.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bxk.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://tns.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hif.jinqigfzy.top

[R34] 退出时清理
来源：http://cyl.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://uoa.guowangkeji.top

[R35] 后台执行并等待
来源：http://iej.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://vze.jinqigufen.top

[R36] 并发执行多个任务
来源：http://wtg.dashuyun.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yku.ctjpmb.com

[R37] 把输出赋给变量
来源：http://jke.tarul.cn

files=$(ls -1)
来源：http://dtp.zhiwuduotai.top

[R38] 管道串联
来源：http://mel.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://uxq.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://svu.yj20258.top

cmd > out.log 2>&1
来源：http://qjo.gaohongyu789.top

[R40] 追加写日志
来源：http://ybi.jqgfzy.top

echo "log" >> out.log
来源：http://shu.sxryk.cn

[R41] 丢弃输出
来源：http://qyg.yonumen.top

cmd >/dev/null 2>&1
来源：http://vma.chenzaomai.com

[R42] 输入重定向
来源：http://nfn.jinghuilouyu.cn

wc -l < a.txt
来源：http://lxl.zhoulong.xyz

[R43] 按名字查找文件
来源：http://drg.fktsv.cn

find . -name "*.log" -type f
来源：http://jcx.zycfv.cn

[R44] 按修改时间查找
来源：http://dix.jianghu66.top

find . -mtime -7 -type f
来源：http://slh.aibaodan.cn

[R45] 批量删除
来源：http://ftq.ydjk.org.cn

find . -name "*.tmp" -delete
来源：http://tdb.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://zvj.zhongyouzk.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ype.haohaochexian.top

[R47] sed 单行替换
来源：http://jzb.haohaochexian.top

sed -i 's/foo/bar/g' a.txt
来源：http://vec.yuxming.cn

[R48] awk 取指定列
来源：http://hvo.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://mtn.smart0.xyz

[R49] awk 带条件
来源：http://sas.bjfxy.top


<!-- 参考信息 -->