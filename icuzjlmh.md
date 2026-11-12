代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://ecn.ehwqpu.com

);
来源：http://ixa.hnxiangtu.top

[Q02] 创建带外键的表
来源：http://dxi.yangfankeji.com

CREATE TABLE orders (
来源：http://fro.shanyushiyangtech.top

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://qgx.sjlbkw.cn

user_id INT NOT NULL,
来源：http://wbw.tianlin.xyz

amount DECIMAL(10, 2),
来源：http://hkw.jinghuilouyu.cn

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://tfu.sufxvd.cn

);
来源：http://ein.wangdashe.top

[Q03] 增加列
来源：http://cct.cucudq.cn

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://uqd.daria6918.cn

[Q04] 修改列类型
来源：http://mzu.hammf.cn

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://uxp.tian-w.cn

[Q05] 重命名列
来源：http://arc.0kj1m.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://vrr.guannengcc.top

[Q06] 删除列
来源：http://ezv.chenlongwang.top

ALTER TABLE users DROP COLUMN age;
来源：http://kcg.ivvv.top

[Q07] 删除表
来源：http://blk.cucudq.cn

DROP TABLE IF EXISTS orders;
来源：http://rhr.zhaomingkeji.xyz

[Q08] 创建普通索引
来源：http://fwu.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qeo.zdqjudy.top

[Q09] 创建唯一索引
来源：http://axl.xuetiantiany.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://rqx.zycfv.cn

[Q10] 插入单行
来源：http://smr.gaohongyu789.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://egu.gzhubu.top

[Q11] 一次插入多行
来源：http://whs.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://rgu.nanxinkj.top

[Q12] 插入后取自增 ID
来源：http://exq.yueranfly.top

INSERT INTO users (name) VALUES ('C');
来源：http://uog.jqgfzy.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://fll.hysaishi.cn

[Q13] 忽略重复插入
来源：http://hck.gzhubu.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://hhq.sufxvd.cn

[Q14] 存在则更新（upsert）
来源：http://xza.zhengqikj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wst.hnxiangtu.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://nss.dianchejie.cn

[Q15] 查询全部
来源：http://fkl.hesvh.cn

SELECT * FROM users;
来源：http://jdm.sjlbkw.cn

[Q16] 查询指定列
来源：http://lvt.chenlongwang.top

SELECT id, name FROM users;
来源：http://dmk.kuanghao11.cn

[Q17] 条件查询
来源：http://aqp.zdbjq.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mzt.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://xuf.zhiwuduotai.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://pvn.zhongyouzk.top

[Q19] 范围查询
来源：http://ubh.ydjk.org.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://nco.yanxiufei.cn

[Q20] IN 列表
来源：http://qqi.pengpengdd.cyou

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pxj.gogol.net.cn

[Q21] 空值判断
来源：http://nbx.sjlbkw.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://eyz.shuidangran.top

[Q22] 排序
来源：http://ats.nwbrower.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qul.yj20258888.top

[Q23] 分页
来源：http://giq.haohaochexian.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xfu.jinghuilouyu.cn

[Q24] 去重
来源：http://ngd.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://hts.epnwcf.com

[Q25] 只取前 N 条
来源：http://sgz.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://slg.fehbvm.com

[Q26] 计数
来源：http://rxb.yfazqb.com

SELECT COUNT(*) FROM users;
来源：http://jlc.havefunace.top

[Q27] 条件计数
来源：http://itb.jianghu66.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://aqn.sysykeji.top

[Q28] 求和与平均
来源：http://zrp.sweek.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://cgx.shangyingyoupin.top

[Q29] 最大最小值
来源：http://djr.uphjek.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://xmp.sweek.top

[Q30] 分组统计
来源：http://xrb.xinyue.icu

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://qon.yj20258.top

[Q31] 分组后过滤
来源：http://izi.nwbrower.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uma.cqqwz.cn

[Q32] 分组拼接字符串
来源：http://okj.316326.xyz

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://ulo.havefunace.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://luo.zhiwuduotai.top

[Q33] 多列分组
来源：http://vlc.chenzaomai.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mzb.epnwcf.com

[Q34] 每组取第一条
来源：http://vzw.9152youxi.cn

SELECT * FROM (
来源：http://xid.sweek.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://adz.jinghuilouyu.cn

) t WHERE rn = 1;
来源：http://mcj.nanxuanxn.top

[Q35] 内连接
来源：http://ruu.ehwqpu.com

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xbg.feifeiyinyue.top

[Q36] 左连接
来源：http://rkf.fehbvm.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://vvk.wangdashe.top

[Q37] 右连接
来源：http://drn.yj20258888.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://bvg.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://kdh.gaohongyu789.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qxj.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://ery.zycfv.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://iha.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wwo.dashuyun.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tjm.ydjk.org.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qvu.guannengcc.top

[Q41] 多表连接
来源：http://zlj.cucudq.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://phj.cheryme.top

JOIN users u ON u.id = o.user_id
来源：http://wfu.gzhubu.top

JOIN products p ON p.id = o.product_id;
来源：http://vpa.jiagoushi.top

[Q42] 连接条件附加过滤
来源：http://zjn.guowangkeji.top

SELECT u.name, o.amount FROM users u
来源：http://kjs.vqdsnc.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://rbd.yj20258888.top

[Q43] 标量子查询
来源：http://oyy.shanyushiyangtech.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://dkt.guannengcc.top

[Q44] IN 子查询
来源：http://vkj.gaohongyu789.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yjo.0kj1m.cn

[Q45] EXISTS 判断存在
来源：http://jky.hammf.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ozl.dashuyun.cn

[Q46] NOT EXISTS 判断不存在
来源：http://umk.fengsongda.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mwv.ehwqpu.com

[Q47] 与平均值比较
来源：http://hzc.ybcxt.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://usu.dianchejie.cn

[Q48] CTE 公用表表达式
来源：http://ekz.zdqjudy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ijp.ppjwa.cn

SELECT * FROM t WHERE c > 5;
来源：http://hif.0kj1m.cn

[Q49] 更新单行
来源：http://ssn.zhengqikj.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qsh.shangyingyoupin.top

[Q50] 批量更新
来源：http://sho.pengpengdd.cyou

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lcf.sufxvd.cn

[Q51] 用子查询更新
来源：http://mrt.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ctn.gaohongyu789.top

[Q52] 删除指定行
来源：http://eow.zhengqikj.top

DELETE FROM users WHERE id = 10;
来源：http://zxp.redwolf501.top

[Q53] 按条件删除
来源：http://hjk.52xcode.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://aoy.fehbvm.com

[Q54] 清空表
来源：http://xlh.guannengcc.top

TRUNCATE TABLE logs;
来源：http://drg.dianchejie.cn

[Q55] 排名（并列占位）
来源：http://edn.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://exg.sweek.top

[Q56] 密集排名（并列不占位）
来源：http://tzs.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bvl.zhongyouzk.top

[Q57] 行号
来源：http://vyx.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fwe.redwolf501.top

[Q58] 累计求和
来源：http://lzs.xylfe.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://osf.redwolf501.top

[Q59] 分组内累计
来源：http://xic.gotoacloud.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yku.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://txl.yonumen.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fco.gotoacloud.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ocu.zhiwuduotai.top

[Q61] 移动平均
来源：http://lnu.dashuyun.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ovq.chenlongwang.top

[Q62] 分组占比
来源：http://aeg.zhixingplan.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dmd.jqgufenzy.top

[Q63] 开启事务
来源：http://dji.nanxuanxn.top

START TRANSACTION;                -- 或 BEGIN
来源：http://dgm.hongshengwenyu.top

[Q64] 提交事务
来源：http://hnc.ivvv.top

COMMIT;
来源：http://iic.kuanghao11.cn

[Q65] 回滚事务
来源：http://asg.guannengcc.top

ROLLBACK;
来源：http://bvf.hesvh.cn

[Q66] 行锁查询
来源：http://rgd.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://sxl.zycfv.cn

[Q67] 设置隔离级别
来源：http://mol.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://isp.fehbvm.com

[Q68] 保存点
来源：http://xdr.xingfuxueyuan.xyz

SAVEPOINT sp1;
来源：http://qrx.sweek.top

ROLLBACK TO sp1;
来源：http://ynj.cashguo.top

[Q69] 查看执行计划
来源：http://ggc.c1oappe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zqx.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://icu.jiagoushi.top

ANALYZE TABLE users;
来源：http://pmq.smart0.xyz

[Q71] 查看建表语句
来源：http://awf.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oac.hnqzz.top

[Q72] 查看索引
来源：http://jve.sysykeji.top

SHOW INDEX FROM users;
来源：http://ygn.guannengcc.top

[Q73] 查看表状态
来源：http://lvm.guowangkeji.top

SHOW TABLE STATUS LIKE 'users';
来源：http://sny.guannengcc.top

[Q74] 强制使用索引
来源：http://uaf.cheryme.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wnn.hysaishi.cn

[Q75] 日期格式化
来源：http://wcn.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://evq.yangfankeji.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ybf.dashuyun.cn

[Q76] 按天统计
来源：http://gla.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iqv.svipenyu.cn

[Q77] 时间加减
来源：http://cdw.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zkn.redwolf501.top

[Q78] 当前时间
来源：http://nse.ppjwa.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sun.wangdashe.top

[Q79] 字符串拼接
来源：http://bfq.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cdw.feifeiyinyue.top

[Q80] 字符串截取
来源：http://mtu.shanyushiyangtech.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vnf.jianghu66.top

[Q81] 字符串替换
来源：http://khx.daria6918.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cuh.bjfxy.top

[Q82] 字符长度与字节长度
来源：http://ums.jinghuilouyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pdf.tanke756.top

[Q83] 大小写转换
来源：http://hjz.shangyingyoupin.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://khv.iojbl.cn

[Q84] 去除首尾空格
来源：http://wer.havefunace.top

SELECT TRIM(name) FROM users;
来源：http://tqc.xuetiantiany.cn

[Q85] 数值取整
来源：http://lcb.cheryme.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fzi.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://vfp.yangfankeji.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ikm.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://yfy.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wia.wangdashe.top

[Q88] 行转列（条件聚合）
来源：http://nfz.pengpengdd.cyou

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bxx.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://csx.pycfn.com

[Q89] 判断表是否存在
来源：http://asy.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fkh.tanke756.top

[Q90] 生成序号列
来源：http://qtp.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://daz.316326.xyz

================================================================================
来源：http://guh.0kj1m.cn

R. Bash 专题
来源：http://zyc.ctjpmb.com

================================================================================
来源：http://mib.tarul.cn

[R01] shebang 与严格模式
来源：http://yhj.tarul.cn

#!/usr/bin/env bash
来源：http://ecl.iojbl.cn

set -euo pipefail
来源：http://oua.xuanzx.com

[R02] 变量赋值与使用
来源：http://pkj.pycfn.com

name="Tom"; echo "$name"
来源：http://khr.pengpengdd.cyou

[R03] 只读变量
来源：http://vge.guowangkeji.top

readonly PI=3.14
来源：http://caf.kuanghao11.cn

[R04] 位置参数
来源：http://dwi.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bom.ydzc1.top

[R05] 参数默认值
来源：http://njq.iojbl.cn

name="${1:-default}"
来源：http://xho.daxiang520.top

[R06] 判断命令是否存在
来源：http://eyc.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lez.yj20258.top

[R07] if 判断文件
来源：http://ilb.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fyb.shangyingyoupin.top

[R08] 数值比较
来源：http://edd.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kfn.hnqzz.top

[R09] 字符串比较
来源：http://qvv.ydjk.org.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://grj.zhijiandao.cn

[R10] 正则匹配
来源：http://ezx.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ocb.jinghuilouyu.cn

[R11] case 多分支
来源：http://syt.jqgfzy.top

case "$1" in
来源：http://zxp.ydzc1.top

start) echo "启动" ;;
来源：http://nuu.ivvv.top

stop)  echo "停止" ;;
来源：http://ksu.fengsongda.top

*)     echo "未知命令" ;;
来源：http://qlt.shangyingyoupin.top

esac
来源：http://frm.c1oappe.top

[R12] for 遍历文件
来源：http://zcn.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://vkp.yangfankeji.com

[R13] for 计数循环
来源：http://glq.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://qoo.quarkkingdee.top

[R14] C 风格 for
来源：http://rcr.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://llj.guannengcc.top

[R15] while 逐行读文件
来源：http://bgw.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mby.c1oappe.top

[R16] until 等待条件
来源：http://eju.zhengqikj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cjh.cqqwz.cn

[R17] 数组定义与取值
来源：http://mtk.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://qrf.cdnleiting.top

[R18] 遍历数组
来源：http://uhg.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wun.zycfv.cn

[R19] 数组长度
来源：http://uol.andypj.xyz

echo "${#arr[@]}"
来源：http://xfc.cucudq.cn

[R20] 关联数组（字典）
来源：http://pqg.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nag.uphjek.com

[R21] 字符串长度
来源：http://vtd.redwolf501.top

echo "${#s}"
来源：http://mhp.hongshengwenyu.top

[R22] 截取子串
来源：http://hqo.ydzc1.top

echo "${s:0:5}"
来源：http://kcg.yanxiufei.cn

[R23] 字符串替换
来源：http://stu.kuanghao11.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rji.jianghu66.top

[R24] 大小写转换
来源：http://itj.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://ddh.yuxming.cn

[R25] 去后缀 / 去前缀
来源：http://ucj.jqgfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vse.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://llt.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://yqz.nanxuanxn.top

[R27] 算术展开
来源：http://mhh.chenzaomai.com

echo $((1 + 2 * 3))
来源：http://pse.jianghu66.top

[R28] 浮点运算
来源：http://dfl.xuetiantiany.cn

echo "scale=2; 10/3" | bc
来源：http://mjj.xziqi.cn

[R29] 定义函数
来源：http://tlv.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fok.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://nwm.fehbvm.com

f() { return 0; }; f || echo "失败了"
来源：http://yvp.daxiang520.top

[R31] 局部变量
来源：http://tuw.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://ays.hnxiangtu.top

[R32] 参数个数校验
来源：http://jea.jlsjyb.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://brz.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://ive.kuanghao11.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mmr.mhx1999.top

[R34] 退出时清理
来源：http://pqr.zdbjq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hwx.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://hjo.jinghuilouyu.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ofw.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://lks.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wyw.ybcxt.top

[R37] 把输出赋给变量
来源：http://gzk.zdqjudy.top

files=$(ls -1)
来源：http://zol.ydjk.org.cn

[R38] 管道串联
来源：http://smr.dashuyun.cn

cat a.txt | grep -i error | wc -l
来源：http://rpk.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://zaz.xinyue.icu

cmd > out.log 2>&1
来源：http://ctc.sweek.top

[R40] 追加写日志
来源：http://jyb.feifeiyinyue.top

echo "log" >> out.log
来源：http://ckp.zdqjudy.top

[R41] 丢弃输出
来源：http://sgr.sxryk.cn

cmd >/dev/null 2>&1
来源：http://hlf.dashuyun.cn

[R42] 输入重定向
来源：http://zwj.zycfv.cn

wc -l < a.txt
来源：http://drb.nanxuanxn.top

[R43] 按名字查找文件
来源：http://xuh.hnqzz.top

find . -name "*.log" -type f
来源：http://eek.mhx1999.top

[R44] 按修改时间查找
来源：http://gfh.haohaochexian.top

find . -mtime -7 -type f
来源：http://jkt.zhaomingkeji.xyz

[R45] 批量删除
来源：http://ikk.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://sjw.yj20258888.top

[R46] 递归替换文件内容
来源：http://ccl.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cip.uphjek.com

[R47] sed 单行替换
来源：http://wms.yvedp.cn


<!-- 参考信息 -->