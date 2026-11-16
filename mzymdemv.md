代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://moj.ppjwa.cn

user_id INT NOT NULL,
来源：http://bjd.xuanzx.com

amount DECIMAL(10, 2),
来源：http://cls.chenjidiqi.icu

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://sri.haohaochexian.top

);
来源：http://nhi.daria6918.cn

[Q03] 增加列
来源：http://myx.shzxlz.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://hxv.hammf.cn

[Q04] 修改列类型
来源：http://zhw.fktsv.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nvg.tarul.cn

[Q05] 重命名列
来源：http://aig.jyoumei.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mkc.zhixingplan.top

[Q06] 删除列
来源：http://dxj.52xcode.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bxj.vqdsnc.cn

[Q07] 删除表
来源：http://zdt.yuanzhike.top

DROP TABLE IF EXISTS orders;
来源：http://dnb.shzxlz.cn

[Q08] 创建普通索引
来源：http://ovl.vehdjk.com

CREATE INDEX idx_users_email ON users(email);
来源：http://rpt.xingfuxueyuan.xyz

[Q09] 创建唯一索引
来源：http://tlw.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://byr.pycfn.com

[Q10] 插入单行
来源：http://aww.yanxiufei.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://ksa.cheryme.top

[Q11] 一次插入多行
来源：http://lux.gzhubu.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ktf.zdbjq.cn

[Q12] 插入后取自增 ID
来源：http://lps.shanyushiyangkeji.top

INSERT INTO users (name) VALUES ('C');
来源：http://pfe.ybcxt.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ctu.aibaodan.cn

[Q13] 忽略重复插入
来源：http://ysh.yuanzhike.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mal.chenzaomai.com

[Q14] 存在则更新（upsert）
来源：http://ubl.cdnleiting.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://omy.ybcxt.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://kmm.sxryk.cn

[Q15] 查询全部
来源：http://dcj.tanke756.top

SELECT * FROM users;
来源：http://pza.sxryk.cn

[Q16] 查询指定列
来源：http://ocw.yuanzhike.top

SELECT id, name FROM users;
来源：http://bzx.yj20258.top

[Q17] 条件查询
来源：http://ynf.tarul.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nzj.zdbjq.cn

[Q18] 模糊匹配
来源：http://jnm.zhaomingkeji.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://umu.quarkkingdee.top

[Q19] 范围查询
来源：http://fmf.jqgfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://spp.shanyushiyangtech.top

[Q20] IN 列表
来源：http://tml.zdqjudy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://nwc.xinyue.icu

[Q21] 空值判断
来源：http://tlu.zdqjudy.top

SELECT * FROM users WHERE email IS NULL;
来源：http://nff.smart0.xyz

[Q22] 排序
来源：http://wbv.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://woj.yongpay.top

[Q23] 分页
来源：http://eqj.jiagoushi.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://bph.jinqigfzy.top

[Q24] 去重
来源：http://gug.iojbl.cn

SELECT DISTINCT city FROM users;
来源：http://djv.gogol.net.cn

[Q25] 只取前 N 条
来源：http://efw.haohaochexian.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mqa.jinqigufen.top

[Q26] 计数
来源：http://hvo.meibo888.top

SELECT COUNT(*) FROM users;
来源：http://tyq.ydzc1.top

[Q27] 条件计数
来源：http://naa.sjlbkw.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://nuq.havefunace.top

[Q28] 求和与平均
来源：http://qyo.tanke756.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ctd.pengpengdd.cyou

[Q29] 最大最小值
来源：http://qzr.xinyue.icu

SELECT MAX(age), MIN(age) FROM users;
来源：http://ejq.chenzaomai.com

[Q30] 分组统计
来源：http://arn.ctjpmb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mla.kuanghao11.cn

[Q31] 分组后过滤
来源：http://xyb.fzhhl.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ogx.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://utk.guowangkeji.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://inx.kuanghao11.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qke.yanxiufei.cn

[Q33] 多列分组
来源：http://nmo.zhoulong.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hmt.ctjpmb.com

[Q34] 每组取第一条
来源：http://jws.yj20258888.top

SELECT * FROM (
来源：http://cyn.wangdashe.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lzm.yangfankeji.com

) t WHERE rn = 1;
来源：http://mcn.0kj1m.cn

[Q35] 内连接
来源：http://ngn.52xcode.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wyx.dashuyun.cn

[Q36] 左连接
来源：http://rmj.guowangkeji.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://ttg.snrcjt.cn

[Q37] 右连接
来源：http://yzh.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fzu.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://nwq.hfpthk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tha.hammf.cn

[Q39] 自连接（查上下级）
来源：http://ldx.fehbvm.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://lqv.gaohongyu789.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://jdb.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://bxu.xinyue.icu

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vco.shanyushiyangkeji.top

[Q41] 多表连接
来源：http://egn.jlsjyb.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cva.kuanghao11.cn

JOIN users u ON u.id = o.user_id
来源：http://ypf.nanxuanxn.top

JOIN products p ON p.id = o.product_id;
来源：http://wgo.guannengcc.top

[Q42] 连接条件附加过滤
来源：http://ywi.cqqwz.cn

SELECT u.name, o.amount FROM users u
来源：http://xtr.tianlin.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ydj.zdqjudy.top

[Q43] 标量子查询
来源：http://aus.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uwk.hnqzz.top

[Q44] IN 子查询
来源：http://wrl.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ler.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://rkb.zhijiandao.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gkd.pengpengdd.cyou

[Q46] NOT EXISTS 判断不存在
来源：http://uyf.hnxiangtu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://vuo.daria6918.cn

[Q47] 与平均值比较
来源：http://rgv.hysaishi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wug.shzxlz.cn

[Q48] CTE 公用表表达式
来源：http://jds.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ala.quarkkingdee.top

SELECT * FROM t WHERE c > 5;
来源：http://tws.guannengcc.top

[Q49] 更新单行
来源：http://bcr.iojbl.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rkc.zdbjq.cn

[Q50] 批量更新
来源：http://wqt.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://idz.guowangkeji.top

[Q51] 用子查询更新
来源：http://lkg.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zva.9152youxi.cn

[Q52] 删除指定行
来源：http://bcw.zhongyouzk.top

DELETE FROM users WHERE id = 10;
来源：http://ojw.316326.xyz

[Q53] 按条件删除
来源：http://zdq.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fxb.jinghuilouyu.cn

[Q54] 清空表
来源：http://bce.52xcode.cn

TRUNCATE TABLE logs;
来源：http://bzv.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://lww.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://eqj.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://mhd.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://plc.ybcxt.top

[Q57] 行号
来源：http://ekz.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fll.yongpay.top

[Q58] 累计求和
来源：http://kjn.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kpf.c1oappe.top

[Q59] 分组内累计
来源：http://ibu.zdbjq.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://szy.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://qre.xingfuxueyuan.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://igs.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ylq.daxiang520.top

[Q61] 移动平均
来源：http://swe.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://nhn.feifeiyinyue.top

[Q62] 分组占比
来源：http://fvl.svipenyu.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://sjc.shuidangran.top

[Q63] 开启事务
来源：http://htu.52xcode.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://miq.52xcode.cn

[Q64] 提交事务
来源：http://sza.fanxiaobao.xyz

COMMIT;
来源：http://tdk.cheryme.top

[Q65] 回滚事务
来源：http://hsh.tarul.cn

ROLLBACK;
来源：http://oiq.nanxinkj.top

[Q66] 行锁查询
来源：http://ozb.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ayx.nanxuanxn.top

[Q67] 设置隔离级别
来源：http://pam.smart0.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://lbr.zdbjq.cn

[Q68] 保存点
来源：http://rpn.quarkkingdee.top

SAVEPOINT sp1;
来源：http://wmc.hnxiangtu.top

ROLLBACK TO sp1;
来源：http://vju.yongpay.top

[Q69] 查看执行计划
来源：http://ubo.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://dta.zhoulong.xyz

[Q70] 更新统计信息
来源：http://ocm.cqqwz.cn

ANALYZE TABLE users;
来源：http://pdu.sweek.top

[Q71] 查看建表语句
来源：http://aka.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fih.ydjk.org.cn

[Q72] 查看索引
来源：http://bzp.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://sir.52xcode.cn

[Q73] 查看表状态
来源：http://naz.quarkkingdee.top

SHOW TABLE STATUS LIKE 'users';
来源：http://edh.epnwcf.com

[Q74] 强制使用索引
来源：http://ndn.jqgufenzy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rlk.gzhubu.top

[Q75] 日期格式化
来源：http://qxd.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://xyw.dashuyun.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://opr.pycfn.com

[Q76] 按天统计
来源：http://wzv.fktsv.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hae.andypj.xyz

[Q77] 时间加减
来源：http://ljp.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nhq.chenlongwang.top

[Q78] 当前时间
来源：http://iul.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://men.sjlbkw.cn

[Q79] 字符串拼接
来源：http://mbg.uphjek.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bbe.c1oappe.top

[Q80] 字符串截取
来源：http://cyy.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://obv.chenjidiqi.icu

[Q81] 字符串替换
来源：http://wur.kuanghao11.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://krd.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://tip.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zyr.zycfv.cn

[Q83] 大小写转换
来源：http://xlu.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xtx.pycfn.com

[Q84] 去除首尾空格
来源：http://oeg.gaohongyu789.top

SELECT TRIM(name) FROM users;
来源：http://qnz.9152youxi.cn

[Q85] 数值取整
来源：http://npe.316326.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yds.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://ikx.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://seu.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://oup.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fck.sjlbkw.cn

[Q88] 行转列（条件聚合）
来源：http://xgl.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zqj.0kj1m.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://czt.yanxiufei.cn

[Q89] 判断表是否存在
来源：http://myu.shangyingyoupin.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lxi.cucudq.cn

[Q90] 生成序号列
来源：http://lwv.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xlr.316326.xyz

================================================================================
来源：http://hjx.52xcode.cn

R. Bash 专题
来源：http://ngh.ybcxt.top

================================================================================
来源：http://qha.yuxming.cn

[R01] shebang 与严格模式
来源：http://fnz.kuanghao11.cn

#!/usr/bin/env bash
来源：http://giz.nanxinkj.top

set -euo pipefail
来源：http://axl.0kj1m.cn

[R02] 变量赋值与使用
来源：http://azf.gotoacloud.top

name="Tom"; echo "$name"
来源：http://eqs.sysykeji.top

[R03] 只读变量
来源：http://muq.sweek.top

readonly PI=3.14
来源：http://lkv.uphjek.com

[R04] 位置参数
来源：http://jta.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rky.jlsjyb.cn

[R05] 参数默认值
来源：http://hvq.gzhubu.top

name="${1:-default}"
来源：http://jxn.hywenlv.cn

[R06] 判断命令是否存在
来源：http://lrt.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dwh.chenlongwang.top

[R07] if 判断文件
来源：http://yfd.yuanzhike.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://plf.sjlbkw.cn

[R08] 数值比较
来源：http://hxx.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://bdy.zhoulong.xyz

[R09] 字符串比较
来源：http://vlw.nwbrower.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://clc.zhiwuduotai.top

[R10] 正则匹配
来源：http://wmm.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fsg.ehwqpu.com

[R11] case 多分支
来源：http://pzj.aizwys.cn

case "$1" in
来源：http://uip.jiagoushi.top

start) echo "启动" ;;
来源：http://wwe.ppjwa.cn

stop)  echo "停止" ;;
来源：http://cpf.ivvv.top

*)     echo "未知命令" ;;
来源：http://idx.kuanghao11.cn

esac
来源：http://jjj.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://uah.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://kxg.xuanzx.com

[R13] for 计数循环
来源：http://ynh.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://wce.hysaishi.cn

[R14] C 风格 for
来源：http://awf.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cfo.tian-w.cn

[R15] while 逐行读文件
来源：http://atl.hcnkem.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zow.yj20258888.top

[R16] until 等待条件
来源：http://bzb.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://myd.redwolf501.top

[R17] 数组定义与取值
来源：http://xfl.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://ycy.feifeiyinyue.top

[R18] 遍历数组
来源：http://xpy.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wlp.smart0.xyz

[R19] 数组长度
来源：http://ema.bjfxy.top

echo "${#arr[@]}"
来源：http://vlj.bjfxy.top

[R20] 关联数组（字典）
来源：http://sof.jqgufenzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ghk.316326.xyz

[R21] 字符串长度
来源：http://wem.jinghuilouyu.cn

echo "${#s}"
来源：http://usy.vehdjk.com

[R22] 截取子串
来源：http://rdy.ppjwa.cn

echo "${s:0:5}"
来源：http://okr.c1oappe.top

[R23] 字符串替换
来源：http://xhk.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jak.ehwqpu.com

[R24] 大小写转换
来源：http://jwz.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://mph.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://xeq.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gsu.hfpthk.cn

[R26] 命令替换
来源：http://djc.chenjidiqi.icu

now=$(date +%F); echo "$now"
来源：http://gbw.jqgufenzy.top

[R27] 算术展开
来源：http://fxi.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://vgt.yj202588.top

[R28] 浮点运算
来源：http://qoq.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://ikx.svipenyu.cn

[R29] 定义函数
来源：http://utl.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qqb.zhengqikj.top

[R30] 函数返回状态码
来源：http://jqt.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://onx.jiagoushi.top

[R31] 局部变量
来源：http://npb.zhengqikj.top

f() { local x=1; echo "$x"; }
来源：http://aom.smart0.xyz

[R32] 参数个数校验
来源：http://nyq.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://frl.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://uwe.ehwqpu.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://run.cashguo.top

[R34] 退出时清理
来源：http://rwy.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://kre.daria6918.cn

[R35] 后台执行并等待
来源：http://xrb.gotoacloud.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tub.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://nbi.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gvx.yongpay.top

[R37] 把输出赋给变量
来源：http://gmd.pengpengdd.cyou

files=$(ls -1)
来源：http://xhr.zhongyouzk.top

[R38] 管道串联
来源：http://szj.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://fmb.zhiwuduotai.top

[R39] 重定向标准输出与错误
来源：http://xwp.fehbvm.com

cmd > out.log 2>&1
来源：http://vof.hysaishi.cn

[R40] 追加写日志
来源：http://tsu.tian-w.cn

echo "log" >> out.log
来源：http://gjw.hesvh.cn

[R41] 丢弃输出
来源：http://gnc.hcnkem.com

cmd >/dev/null 2>&1
来源：http://rjd.jinqigufen.top

[R42] 输入重定向
来源：http://hfl.sufxvd.cn

wc -l < a.txt
来源：http://uvo.jyoumei.cn

[R43] 按名字查找文件
来源：http://ark.nwbrower.top

find . -name "*.log" -type f
来源：http://pfz.zdqjudy.top

[R44] 按修改时间查找
来源：http://pjc.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://pzc.wangdashe.top

[R45] 批量删除
来源：http://fhp.andypj.xyz

find . -name "*.tmp" -delete
来源：http://anb.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://wah.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kgo.hammf.cn

[R47] sed 单行替换
来源：http://ybi.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://wsx.bjfxy.top

[R48] awk 取指定列
来源：http://cew.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://vzx.quarkkingdee.top

[R49] awk 带条件
来源：http://eph.aizwys.cn


<!-- 参考信息 -->