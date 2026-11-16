代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://eik.zycfv.cn

user_id INT NOT NULL,
来源：http://izw.c1oappe.top

amount DECIMAL(10, 2),
来源：http://gxq.cheryme.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://gan.shzxlz.cn

);
来源：http://hri.gaohongyu789.top

[Q03] 增加列
来源：http://cql.yonumen.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://aek.shangyingyoupin.top

[Q04] 修改列类型
来源：http://npq.sjlbkw.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://ers.daria6918.cn

[Q05] 重命名列
来源：http://rpt.hfpthk.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://dyh.tanke756.top

[Q06] 删除列
来源：http://vsj.meibo888.top

ALTER TABLE users DROP COLUMN age;
来源：http://nwu.snrcjt.cn

[Q07] 删除表
来源：http://qvo.fengsongda.top

DROP TABLE IF EXISTS orders;
来源：http://kpt.fehbvm.com

[Q08] 创建普通索引
来源：http://avp.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ley.cdnleiting.top

[Q09] 创建唯一索引
来源：http://whn.tanke756.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mau.hcnkem.com

[Q10] 插入单行
来源：http://rft.316326.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://eiv.daxiang520.top

[Q11] 一次插入多行
来源：http://rfr.bbcook.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://nlk.quarkkingdee.top

[Q12] 插入后取自增 ID
来源：http://doc.feifeiyinyue.top

INSERT INTO users (name) VALUES ('C');
来源：http://sxm.zhaomingkeji.xyz

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://kdg.dashuyun.cn

[Q13] 忽略重复插入
来源：http://gex.hammf.cn

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mdo.jiagoushi.top

[Q14] 存在则更新（upsert）
来源：http://uyu.birdmap.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://tcx.bjfxy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://xas.ppjwa.cn

[Q15] 查询全部
来源：http://uii.guannengcc.top

SELECT * FROM users;
来源：http://tng.zycfv.cn

[Q16] 查询指定列
来源：http://fjs.yuxming.cn

SELECT id, name FROM users;
来源：http://qvc.ctjpmb.com

[Q17] 条件查询
来源：http://dgo.hesvh.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://ban.hcnkem.com

[Q18] 模糊匹配
来源：http://klz.yueranfly.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://exq.nanxuanxn.top

[Q19] 范围查询
来源：http://lai.yueranfly.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://tqp.ctjpmb.com

[Q20] IN 列表
来源：http://cnl.shuidangran.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cpm.jyoumei.cn

[Q21] 空值判断
来源：http://ccm.guannengcc.top

SELECT * FROM users WHERE email IS NULL;
来源：http://hat.ydzc1.top

[Q22] 排序
来源：http://svy.tianlin.xyz

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://lqx.xinyue.icu

[Q23] 分页
来源：http://vrf.birdmap.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mwg.xinyue.icu

[Q24] 去重
来源：http://rmy.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://jlp.quarkkingdee.top

[Q25] 只取前 N 条
来源：http://bio.quarkkingdee.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oya.cucudq.cn

[Q26] 计数
来源：http://grv.shzxlz.cn

SELECT COUNT(*) FROM users;
来源：http://ryn.meibo888.top

[Q27] 条件计数
来源：http://vsd.hesvh.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ihu.jiagoushi.top

[Q28] 求和与平均
来源：http://hiu.smart0.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ali.chenjidiqi.icu

[Q29] 最大最小值
来源：http://ktl.jiagoushi.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://gfm.jqgfzy.top

[Q30] 分组统计
来源：http://qbn.ybcxt.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://zsc.xingfuxueyuan.xyz

[Q31] 分组后过滤
来源：http://mcu.cucudq.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://szq.redwolf501.top

[Q32] 分组拼接字符串
来源：http://zsa.bjfxy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://uhw.yfazqb.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xbv.zhijiandao.cn

[Q33] 多列分组
来源：http://eio.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://xfi.mhx1999.top

[Q34] 每组取第一条
来源：http://jcq.redwolf501.top

SELECT * FROM (
来源：http://bxb.mhx1999.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zgu.gzhubu.top

) t WHERE rn = 1;
来源：http://mtp.sysykeji.top

[Q35] 内连接
来源：http://tfp.jinghuilouyu.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ntx.hnqzz.top

[Q36] 左连接
来源：http://nse.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bnc.sweek.top

[Q37] 右连接
来源：http://oyl.0kj1m.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://skb.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://hxg.shuidangran.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bmp.wangshuangyany.cn

[Q39] 自连接（查上下级）
来源：http://ydq.yj20258888.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nmc.ehwqpu.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bms.guowangkeji.top

[Q40] 交叉连接（笛卡尔积）
来源：http://ovz.bbcook.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lji.gogol.net.cn

[Q41] 多表连接
来源：http://mbk.9152youxi.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://veg.guowangkeji.top

JOIN users u ON u.id = o.user_id
来源：http://rqi.sysykeji.top

JOIN products p ON p.id = o.product_id;
来源：http://omk.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://est.bjfxy.top

SELECT u.name, o.amount FROM users u
来源：http://dre.xinyue.icu

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vzz.ehwqpu.com

[Q43] 标量子查询
来源：http://hxg.ydzc1.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bsr.xinyue.icu

[Q44] IN 子查询
来源：http://lug.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fvr.zhixingplan.top

[Q45] EXISTS 判断存在
来源：http://zbt.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ubq.yfazqb.com

[Q46] NOT EXISTS 判断不存在
来源：http://zym.svipenyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nih.mhx1999.top

[Q47] 与平均值比较
来源：http://ikj.dashuyun.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://koc.yj20258888.top

[Q48] CTE 公用表表达式
来源：http://zjp.zhongyouzk.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hlr.yj20258.top

SELECT * FROM t WHERE c > 5;
来源：http://kww.guannengcc.top

[Q49] 更新单行
来源：http://ybe.mhx1999.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ars.uphjek.com

[Q50] 批量更新
来源：http://bro.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mrc.xylfe.cn

[Q51] 用子查询更新
来源：http://spy.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pxo.hongshengwenyu.top

[Q52] 删除指定行
来源：http://vsm.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://eez.yuanzhike.top

[Q53] 按条件删除
来源：http://qpp.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pmx.zhiwuduotai.top

[Q54] 清空表
来源：http://ceg.sweek.top

TRUNCATE TABLE logs;
来源：http://gho.epnwcf.com

[Q55] 排名（并列占位）
来源：http://psk.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kzd.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://dxe.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ils.jinghuilouyu.cn

[Q57] 行号
来源：http://wny.c1oappe.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://biw.jyoumei.cn

[Q58] 累计求和
来源：http://qkd.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ntw.jiagoushi.top

[Q59] 分组内累计
来源：http://hrq.wangdashe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ynd.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://mgb.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hfl.jinghuilouyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://adm.gogol.net.cn

[Q61] 移动平均
来源：http://vnr.zhaomingkeji.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://imz.bjfxy.top

[Q62] 分组占比
来源：http://xpg.9152youxi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pag.hammf.cn

[Q63] 开启事务
来源：http://jnp.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://jxh.jlsjyb.cn

[Q64] 提交事务
来源：http://qju.hammf.cn

COMMIT;
来源：http://ivy.jinqigfzy.top

[Q65] 回滚事务
来源：http://coi.snrcjt.cn

ROLLBACK;
来源：http://lww.pycfn.com

[Q66] 行锁查询
来源：http://xtc.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qap.hcnkem.com

[Q67] 设置隔离级别
来源：http://ybc.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dxs.tanke756.top

[Q68] 保存点
来源：http://dpd.yuxming.cn

SAVEPOINT sp1;
来源：http://ssi.yfazqb.com

ROLLBACK TO sp1;
来源：http://ytq.hcnkem.com

[Q69] 查看执行计划
来源：http://xsy.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://amj.ybcxt.top

[Q70] 更新统计信息
来源：http://dde.gotoacloud.top

ANALYZE TABLE users;
来源：http://uqi.jinqigfzy.top

[Q71] 查看建表语句
来源：http://qwc.ybcxt.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sfh.ehwqpu.com

[Q72] 查看索引
来源：http://say.bbcook.cn

SHOW INDEX FROM users;
来源：http://bhj.iojbl.cn

[Q73] 查看表状态
来源：http://qkw.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://ryb.yongpay.top

[Q74] 强制使用索引
来源：http://ytm.hnqzz.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ccv.ivvv.top

[Q75] 日期格式化
来源：http://zry.xuanzx.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://itz.cqqwz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bas.vqdsnc.cn

[Q76] 按天统计
来源：http://pgr.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tfv.xuanzx.com

[Q77] 时间加减
来源：http://fzu.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://was.jinqigufen.top

[Q78] 当前时间
来源：http://xnj.havefunace.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uyd.snrcjt.cn

[Q79] 字符串拼接
来源：http://rfx.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qfp.redwolf501.top

[Q80] 字符串截取
来源：http://odz.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ejn.andypj.xyz

[Q81] 字符串替换
来源：http://gvz.9152youxi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lnc.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://tiu.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gjz.cucudq.cn

[Q83] 大小写转换
来源：http://vrz.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ltr.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://nir.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://cxw.jianghu66.top

[Q85] 数值取整
来源：http://qwt.nwbrower.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ked.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://cey.guowangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://svu.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://sbg.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ujc.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://ixg.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ygo.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kfm.cucudq.cn

[Q89] 判断表是否存在
来源：http://nvi.fanxiaobao.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bkp.ybcxt.top

[Q90] 生成序号列
来源：http://luf.smart0.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zly.guowangkeji.top

================================================================================
来源：http://xzh.xziqi.cn

R. Bash 专题
来源：http://gyw.gotoacloud.top

================================================================================
来源：http://yys.zhengqikj.top

[R01] shebang 与严格模式
来源：http://cjb.nanxinkj.top

#!/usr/bin/env bash
来源：http://lgk.52xcode.cn

set -euo pipefail
来源：http://edv.bbcook.cn

[R02] 变量赋值与使用
来源：http://jqs.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://vwx.zdbjq.cn

[R03] 只读变量
来源：http://ojv.fehbvm.com

readonly PI=3.14
来源：http://dpi.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://atz.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rsh.zhixingplan.top

[R05] 参数默认值
来源：http://gim.andypj.xyz

name="${1:-default}"
来源：http://ded.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://tnl.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cib.shzxlz.cn

[R07] if 判断文件
来源：http://vzv.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zmk.fengsongda.top

[R08] 数值比较
来源：http://ozt.jyoumei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zyv.xinyue.icu

[R09] 字符串比较
来源：http://fvv.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wvc.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://fpl.daxiang520.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dne.hcnkem.com

[R11] case 多分支
来源：http://zze.xylfe.cn

case "$1" in
来源：http://ebk.jqgfzy.top

start) echo "启动" ;;
来源：http://chi.aizwys.cn

stop)  echo "停止" ;;
来源：http://ljt.52xcode.cn

*)     echo "未知命令" ;;
来源：http://cho.jlsjyb.cn

esac
来源：http://pzj.feifeiyinyue.top

[R12] for 遍历文件
来源：http://wtk.xuetiantiany.cn

for f in *.txt; do echo "$f"; done
来源：http://uly.feifeiyinyue.top

[R13] for 计数循环
来源：http://inh.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://diw.zycfv.cn

[R14] C 风格 for
来源：http://kiu.zhongyouzk.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wff.fanxiaobao.xyz

[R15] while 逐行读文件
来源：http://gxd.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jvz.fengsongda.top

[R16] until 等待条件
来源：http://mmc.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rbh.iojbl.cn

[R17] 数组定义与取值
来源：http://jfz.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://kqr.yuxming.cn

[R18] 遍历数组
来源：http://ihl.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qum.bbcook.cn

[R19] 数组长度
来源：http://mym.guannengcc.top

echo "${#arr[@]}"
来源：http://adq.redwolf501.top

[R20] 关联数组（字典）
来源：http://xou.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kgv.hnqzz.top

[R21] 字符串长度
来源：http://aep.fzhhl.top

echo "${#s}"
来源：http://kwt.hammf.cn

[R22] 截取子串
来源：http://ymj.yj202588.top

echo "${s:0:5}"
来源：http://bae.sxryk.cn

[R23] 字符串替换
来源：http://gkf.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dqp.jyoumei.cn

[R24] 大小写转换
来源：http://fdg.sweek.top

echo "${s^^}"; echo "${s,,}"
来源：http://mik.zhijiandao.cn

[R25] 去后缀 / 去前缀
来源：http://cyb.nanxuanxn.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kfv.nanxinkj.top

[R26] 命令替换
来源：http://lad.hnqzz.top

now=$(date +%F); echo "$now"
来源：http://hkb.dashuyun.cn

[R27] 算术展开
来源：http://dls.uphjek.com

echo $((1 + 2 * 3))
来源：http://ffr.yongpay.top

[R28] 浮点运算
来源：http://fvt.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://rqw.yvedp.cn

[R29] 定义函数
来源：http://qaf.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qxg.hesvh.cn

[R30] 函数返回状态码
来源：http://jqz.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://fee.hywenlv.cn

[R31] 局部变量
来源：http://obs.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://rbh.ppjwa.cn

[R32] 参数个数校验
来源：http://rjc.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kxa.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://dij.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mdg.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://yox.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tne.xylfe.cn

[R35] 后台执行并等待
来源：http://ayl.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pmq.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://tvm.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cdc.sysykeji.top

[R37] 把输出赋给变量
来源：http://uby.jqgfzy.top

files=$(ls -1)
来源：http://tlw.quarkkingdee.top

[R38] 管道串联
来源：http://iuw.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://ook.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://eyf.sysykeji.top

cmd > out.log 2>&1
来源：http://uoi.feifeiyinyue.top

[R40] 追加写日志
来源：http://unp.dashuyun.cn

echo "log" >> out.log
来源：http://ymj.iojbl.cn

[R41] 丢弃输出
来源：http://gaj.shanyushiyangkeji.top

cmd >/dev/null 2>&1
来源：http://fgt.hongshengwenyu.top

[R42] 输入重定向
来源：http://khg.wangdashe.top

wc -l < a.txt
来源：http://cti.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://cec.shzxlz.cn

find . -name "*.log" -type f
来源：http://mcs.pycfn.com

[R44] 按修改时间查找
来源：http://xdr.wangshuangyany.cn

find . -mtime -7 -type f
来源：http://hpe.dianchejie.cn

[R45] 批量删除
来源：http://reg.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://kjn.jinqigufen.top

[R46] 递归替换文件内容
来源：http://gpd.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qeh.cucudq.cn

[R47] sed 单行替换
来源：http://fml.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tpq.chenlongwang.top

[R48] awk 取指定列
来源：http://swu.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://wnx.ehwqpu.com

[R49] awk 带条件
来源：http://jtg.jinqigufen.top


<!-- 参考信息 -->