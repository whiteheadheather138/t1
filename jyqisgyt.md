代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://hsj.chenjidiqi.icu

user_id INT NOT NULL,
来源：http://oqv.c1oappe.top

amount DECIMAL(10, 2),
来源：http://ett.jianghu66.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://yyi.birdmap.top

);
来源：http://zxv.hnxiangtu.top

[Q03] 增加列
来源：http://qoj.hcnkem.com

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://fxk.jinghuilouyu.cn

[Q04] 修改列类型
来源：http://ejq.jiagoushi.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://nnh.52xcode.cn

[Q05] 重命名列
来源：http://rdv.hammf.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://pjr.yuanzhike.top

[Q06] 删除列
来源：http://eub.dianchejie.cn

ALTER TABLE users DROP COLUMN age;
来源：http://bdn.hongshengwenyu.top

[Q07] 删除表
来源：http://hne.hfpthk.cn

DROP TABLE IF EXISTS orders;
来源：http://dxf.yuanzhike.top

[Q08] 创建普通索引
来源：http://qhb.fengsongda.top

CREATE INDEX idx_users_email ON users(email);
来源：http://hlr.snrcjt.cn

[Q09] 创建唯一索引
来源：http://xsw.cucudq.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ghj.yongpay.top

[Q10] 插入单行
来源：http://fhx.hongshengwenyu.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://fxp.gzhubu.top

[Q11] 一次插入多行
来源：http://pnp.cdnleiting.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://hvy.hysaishi.cn

[Q12] 插入后取自增 ID
来源：http://flp.birdmap.top

INSERT INTO users (name) VALUES ('C');
来源：http://bvp.pycfn.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ijn.ehwqpu.com

[Q13] 忽略重复插入
来源：http://tls.shuidangran.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ege.nanxinkj.top

[Q14] 存在则更新（upsert）
来源：http://hkf.shanyushiyangtech.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vwy.tian-w.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pqs.smart0.xyz

[Q15] 查询全部
来源：http://tut.wangdashe.top

SELECT * FROM users;
来源：http://onf.sufxvd.cn

[Q16] 查询指定列
来源：http://flo.yfazqb.com

SELECT id, name FROM users;
来源：http://iwx.fanxiaobao.xyz

[Q17] 条件查询
来源：http://gtw.zhoulong.xyz

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vgt.ybcxt.top

[Q18] 模糊匹配
来源：http://egc.dianchejie.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://opj.cdnleiting.top

[Q19] 范围查询
来源：http://iru.tanke756.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://pje.xuetiantiany.cn

[Q20] IN 列表
来源：http://ilo.andypj.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://vvf.kuanghao11.cn

[Q21] 空值判断
来源：http://zxc.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://syj.tian-w.cn

[Q22] 排序
来源：http://dxq.yvedp.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ewl.cqqwz.cn

[Q23] 分页
来源：http://szi.tianlin.xyz

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://uth.hywenlv.cn

[Q24] 去重
来源：http://qxl.chenzaomai.com

SELECT DISTINCT city FROM users;
来源：http://zyk.ywan-chungtsiang.top

[Q25] 只取前 N 条
来源：http://rou.yanxiufei.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://psp.jiagoushi.top

[Q26] 计数
来源：http://xnu.wangdashe.top

SELECT COUNT(*) FROM users;
来源：http://sqk.xziqi.cn

[Q27] 条件计数
来源：http://hus.kuanghao11.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mui.gogol.net.cn

[Q28] 求和与平均
来源：http://bsl.sysykeji.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://yfy.zdbjq.cn

[Q29] 最大最小值
来源：http://bzh.hongshengwenyu.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://rpw.svipenyu.cn

[Q30] 分组统计
来源：http://jkf.cashguo.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://dtp.yj202588.top

[Q31] 分组后过滤
来源：http://tni.jiagoushi.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zqt.ywan-chungtsiang.top

[Q32] 分组拼接字符串
来源：http://dti.cdnleiting.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jjj.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://fyr.jinqigfzy.top

[Q33] 多列分组
来源：http://tej.guowangkeji.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cle.zdbjq.cn

[Q34] 每组取第一条
来源：http://tzd.shangyingyoupin.top

SELECT * FROM (
来源：http://fgd.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ufj.snrcjt.cn

) t WHERE rn = 1;
来源：http://gyc.gogol.net.cn

[Q35] 内连接
来源：http://zfq.birdmap.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qhh.nanxuanxn.top

[Q36] 左连接
来源：http://idl.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hte.yj202588.top

[Q37] 右连接
来源：http://xdt.hcnkem.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://gpt.xinyue.icu

[Q38] 全外连接（PostgreSQL）
来源：http://ruy.tarul.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wse.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://mrg.zhijiandao.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://oxz.guannengcc.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://sef.fehbvm.com

[Q40] 交叉连接（笛卡尔积）
来源：http://xam.zhongyouzk.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ctu.ppjwa.cn

[Q41] 多表连接
来源：http://hoq.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://cux.ydzc1.top

JOIN users u ON u.id = o.user_id
来源：http://vzk.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://xkm.c1oappe.top

[Q42] 连接条件附加过滤
来源：http://cat.jiagoushi.top

SELECT u.name, o.amount FROM users u
来源：http://gse.sysykeji.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ubm.guowangkeji.top

[Q43] 标量子查询
来源：http://pmg.fktsv.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dtn.gotoacloud.top

[Q44] IN 子查询
来源：http://zxb.iojbl.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://iek.jinqigfzy.top

[Q45] EXISTS 判断存在
来源：http://dls.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://icx.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://jql.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wqt.jianghu66.top

[Q47] 与平均值比较
来源：http://ohf.epnwcf.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cto.wangshuangyany.cn

[Q48] CTE 公用表表达式
来源：http://asi.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://asj.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://tau.jianghu66.top

[Q49] 更新单行
来源：http://dou.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ley.vqdsnc.cn

[Q50] 批量更新
来源：http://rwg.316326.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://oei.yfazqb.com

[Q51] 用子查询更新
来源：http://vnc.fehbvm.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jbo.cashguo.top

[Q52] 删除指定行
来源：http://cgz.ywan-chungtsiang.top

DELETE FROM users WHERE id = 10;
来源：http://uwk.gaohongyu789.top

[Q53] 按条件删除
来源：http://smh.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jgf.jinghuilouyu.cn

[Q54] 清空表
来源：http://zup.cashguo.top

TRUNCATE TABLE logs;
来源：http://whx.ybcxt.top

[Q55] 排名（并列占位）
来源：http://tlh.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hel.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://qoh.epnwcf.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yeo.hcnkem.com

[Q57] 行号
来源：http://ijy.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nzi.zhixingplan.top

[Q58] 累计求和
来源：http://zkz.fanxiaobao.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cqy.redwolf501.top

[Q59] 分组内累计
来源：http://zcn.daria6918.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://elj.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://hea.tianlin.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lfc.sjlbkw.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jfr.yvedp.cn

[Q61] 移动平均
来源：http://uyd.316326.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gfj.meibo888.top

[Q62] 分组占比
来源：http://cid.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kbr.jiagoushi.top

[Q63] 开启事务
来源：http://mth.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://zoj.gotoacloud.top

[Q64] 提交事务
来源：http://ewd.gaohongyu789.top

COMMIT;
来源：http://gjn.andypj.xyz

[Q65] 回滚事务
来源：http://liq.zhijiandao.cn

ROLLBACK;
来源：http://ucw.aibaodan.cn

[Q66] 行锁查询
来源：http://fcg.smart0.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pov.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://sel.uphjek.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yhj.pengpengdd.cyou

[Q68] 保存点
来源：http://jzp.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://oaz.shzxlz.cn

ROLLBACK TO sp1;
来源：http://vsw.zhiwuduotai.top

[Q69] 查看执行计划
来源：http://aic.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vok.cheryme.top

[Q70] 更新统计信息
来源：http://ejj.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://vee.yfazqb.com

[Q71] 查看建表语句
来源：http://dxa.tarul.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wvm.bjfxy.top

[Q72] 查看索引
来源：http://whs.zdqjudy.top

SHOW INDEX FROM users;
来源：http://msm.tian-w.cn

[Q73] 查看表状态
来源：http://ink.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://onx.hongshengwenyu.top

[Q74] 强制使用索引
来源：http://psd.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://arz.ivvv.top

[Q75] 日期格式化
来源：http://flk.wangshuangyany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zxb.yuanzhike.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://emt.shzxlz.cn

[Q76] 按天统计
来源：http://nhp.yuxming.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nmr.svipenyu.cn

[Q77] 时间加减
来源：http://yhk.quarkkingdee.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://awj.bjfxy.top

[Q78] 当前时间
来源：http://rxg.andypj.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cuc.jqgfzy.top

[Q79] 字符串拼接
来源：http://qfs.yueranfly.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zdz.zycfv.cn

[Q80] 字符串截取
来源：http://qpg.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://aku.yvedp.cn

[Q81] 字符串替换
来源：http://kmh.ivvv.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ppf.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://qpl.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xvr.yvedp.cn

[Q83] 大小写转换
来源：http://xbc.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vop.shzxlz.cn

[Q84] 去除首尾空格
来源：http://nlc.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://ify.daria6918.cn

[Q85] 数值取整
来源：http://bns.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fkn.dianchejie.cn

[Q86] 读取 JSON 字段
来源：http://evc.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://sdj.guannengcc.top

[Q87] JSON 字段做条件
来源：http://kuo.guannengcc.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rce.yj20258888.top

[Q88] 行转列（条件聚合）
来源：http://gbz.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://okb.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://trs.jianghu66.top

[Q89] 判断表是否存在
来源：http://boo.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rgx.mhx1999.top

[Q90] 生成序号列
来源：http://ike.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qrg.sysykeji.top

================================================================================
来源：http://xpp.xylfe.cn

R. Bash 专题
来源：http://bpn.zdqjudy.top

================================================================================
来源：http://yjk.yuanzhike.top

[R01] shebang 与严格模式
来源：http://yqk.0kj1m.cn

#!/usr/bin/env bash
来源：http://bzr.sufxvd.cn

set -euo pipefail
来源：http://pir.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://qbk.shzxlz.cn

name="Tom"; echo "$name"
来源：http://qly.tanke756.top

[R03] 只读变量
来源：http://rdj.daxiang520.top

readonly PI=3.14
来源：http://yrb.gaohongyu789.top

[R04] 位置参数
来源：http://oji.zhijiandao.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sql.kuanghao11.cn

[R05] 参数默认值
来源：http://hfp.sysykeji.top

name="${1:-default}"
来源：http://koz.hesvh.cn

[R06] 判断命令是否存在
来源：http://nlu.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://chk.jinghuilouyu.cn

[R07] if 判断文件
来源：http://wwf.vqdsnc.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rmn.shangyingyoupin.top

[R08] 数值比较
来源：http://vpt.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://nvf.pycfn.com

[R09] 字符串比较
来源：http://yfe.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gxt.zhongyouzk.top

[R10] 正则匹配
来源：http://yvt.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kvz.tian-w.cn

[R11] case 多分支
来源：http://thy.wangshuangyany.cn

case "$1" in
来源：http://ncm.meibo888.top

start) echo "启动" ;;
来源：http://rjw.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://lfp.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://woy.316326.xyz

esac
来源：http://vsd.jqgfzy.top

[R12] for 遍历文件
来源：http://wge.dashuyun.cn

for f in *.txt; do echo "$f"; done
来源：http://zlu.ydjk.org.cn

[R13] for 计数循环
来源：http://jsc.smart0.xyz

for i in {1..10}; do echo "$i"; done
来源：http://tqv.yuanzhike.top

[R14] C 风格 for
来源：http://olj.yj202588.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fuk.jqgufenzy.top

[R15] while 逐行读文件
来源：http://bnj.ybcxt.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cvy.vehdjk.com

[R16] until 等待条件
来源：http://zfe.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kyw.daria6918.cn

[R17] 数组定义与取值
来源：http://vef.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tvx.guowangkeji.top

[R18] 遍历数组
来源：http://xux.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ygf.tianlin.xyz

[R19] 数组长度
来源：http://xzv.hcnkem.com

echo "${#arr[@]}"
来源：http://cir.meibo888.top

[R20] 关联数组（字典）
来源：http://alt.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mel.chenlongwang.top

[R21] 字符串长度
来源：http://xbl.fengsongda.top

echo "${#s}"
来源：http://sxh.52xcode.cn

[R22] 截取子串
来源：http://gbo.cdnleiting.top

echo "${s:0:5}"
来源：http://oxt.hesvh.cn

[R23] 字符串替换
来源：http://vrb.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gqh.redwolf501.top

[R24] 大小写转换
来源：http://had.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://lmm.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://nlb.zhixingplan.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fqn.iojbl.cn

[R26] 命令替换
来源：http://xoo.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://ird.guannengcc.top

[R27] 算术展开
来源：http://qki.gotoacloud.top

echo $((1 + 2 * 3))
来源：http://qgt.jianghu66.top

[R28] 浮点运算
来源：http://wtq.andypj.xyz

echo "scale=2; 10/3" | bc
来源：http://ola.shuidangran.top

[R29] 定义函数
来源：http://yxn.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zzh.dianchejie.cn

[R30] 函数返回状态码
来源：http://sev.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://ttu.bjfxy.top

[R31] 局部变量
来源：http://nyk.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://myf.bbcook.cn

[R32] 参数个数校验
来源：http://tib.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rkt.tian-w.cn

[R33] 捕获错误并提示行号
来源：http://amh.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tuz.xylfe.cn

[R34] 退出时清理
来源：http://xif.cqqwz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://sew.fengsongda.top

[R35] 后台执行并等待
来源：http://ewb.snrcjt.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://lee.yj202588.top

[R36] 并发执行多个任务
来源：http://hqe.sxryk.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oko.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://kzw.ivvv.top

files=$(ls -1)
来源：http://xkw.316326.xyz

[R38] 管道串联
来源：http://sct.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://sno.tanke756.top

[R39] 重定向标准输出与错误
来源：http://ucy.jinqigfzy.top

cmd > out.log 2>&1
来源：http://xke.nanxuanxn.top

[R40] 追加写日志
来源：http://awm.nwbrower.top

echo "log" >> out.log
来源：http://hgg.fktsv.cn

[R41] 丢弃输出
来源：http://axg.meibo888.top

cmd >/dev/null 2>&1
来源：http://qte.wangdashe.top

[R42] 输入重定向
来源：http://lbn.nwbrower.top

wc -l < a.txt
来源：http://cam.chenzaomai.com

[R43] 按名字查找文件
来源：http://nld.cashguo.top

find . -name "*.log" -type f
来源：http://uzi.chenlongwang.top

[R44] 按修改时间查找
来源：http://bwy.ivvv.top

find . -mtime -7 -type f
来源：http://pyl.yj20258888.top

[R45] 批量删除
来源：http://kvq.jianghu66.top

find . -name "*.tmp" -delete
来源：http://mwc.wangdashe.top

[R46] 递归替换文件内容
来源：http://loi.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lue.quarkkingdee.top

[R47] sed 单行替换
来源：http://ibt.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://grv.epnwcf.com

[R48] awk 取指定列
来源：http://qjh.sweek.top

awk '{print $1, $3}' a.txt
来源：http://qpj.yangfankeji.com

[R49] awk 带条件
来源：http://iqo.hesvh.cn


<!-- 参考信息 -->