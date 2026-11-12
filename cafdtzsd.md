代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://ang.xylfe.cn

user_id INT NOT NULL,
来源：http://qzr.ivvv.top

amount DECIMAL(10, 2),
来源：http://zav.jinqigfzy.top

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://lqs.aizwys.cn

);
来源：http://qmt.ydzc1.top

[Q03] 增加列
来源：http://gax.mhx1999.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://meh.nanxuanxn.top

[Q04] 修改列类型
来源：http://mgz.yj20258.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vlu.tian-w.cn

[Q05] 重命名列
来源：http://wit.pycfn.com

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://ydo.ivvv.top

[Q06] 删除列
来源：http://alq.pycfn.com

ALTER TABLE users DROP COLUMN age;
来源：http://hwx.xuetiantiany.cn

[Q07] 删除表
来源：http://soh.hammf.cn

DROP TABLE IF EXISTS orders;
来源：http://lxr.ppjwa.cn

[Q08] 创建普通索引
来源：http://har.sjlbkw.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://xjx.yfazqb.com

[Q09] 创建唯一索引
来源：http://sbd.tianlin.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://pwr.xinyue.icu

[Q10] 插入单行
来源：http://psn.jianghu66.top

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://hmu.havefunace.top

[Q11] 一次插入多行
来源：http://xds.xziqi.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://qhc.316326.xyz

[Q12] 插入后取自增 ID
来源：http://rhm.ywan-chungtsiang.top

INSERT INTO users (name) VALUES ('C');
来源：http://syp.yongpay.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://awa.cashguo.top

[Q13] 忽略重复插入
来源：http://pup.nwbrower.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bmw.52xcode.cn

[Q14] 存在则更新（upsert）
来源：http://tur.9152youxi.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://vxd.jqgfzy.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://zth.hongshengwenyu.top

[Q15] 查询全部
来源：http://rgs.chenjidiqi.icu

SELECT * FROM users;
来源：http://pyw.hysaishi.cn

[Q16] 查询指定列
来源：http://lns.xuanzx.com

SELECT id, name FROM users;
来源：http://cet.ybcxt.top

[Q17] 条件查询
来源：http://yuc.bjfxy.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://qwt.epnwcf.com

[Q18] 模糊匹配
来源：http://hpe.ehwqpu.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://vzs.hfpthk.cn

[Q19] 范围查询
来源：http://wbh.xuanzx.com

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://two.daxiang520.top

[Q20] IN 列表
来源：http://vkb.gaohongyu789.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://urr.tian-w.cn

[Q21] 空值判断
来源：http://pot.fzhhl.top

SELECT * FROM users WHERE email IS NULL;
来源：http://rjd.gogol.net.cn

[Q22] 排序
来源：http://spu.yj202588.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://ymp.yangfankeji.com

[Q23] 分页
来源：http://ahb.ctjpmb.com

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://pnm.jinghuilouyu.cn

[Q24] 去重
来源：http://aks.shanyushiyangkeji.top

SELECT DISTINCT city FROM users;
来源：http://pcz.bjfxy.top

[Q25] 只取前 N 条
来源：http://mhn.aibaodan.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://knw.shangyingyoupin.top

[Q26] 计数
来源：http://ioj.316326.xyz

SELECT COUNT(*) FROM users;
来源：http://eui.feifeiyinyue.top

[Q27] 条件计数
来源：http://krg.hnxiangtu.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://cyp.daxiang520.top

[Q28] 求和与平均
来源：http://aep.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blp.52xcode.cn

[Q29] 最大最小值
来源：http://vap.hysaishi.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://hrz.xuetiantiany.cn

[Q30] 分组统计
来源：http://jpt.shangyingyoupin.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vcu.jinghuilouyu.cn

[Q31] 分组后过滤
来源：http://xla.yonumen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gsx.ivvv.top

[Q32] 分组拼接字符串
来源：http://xho.hcnkem.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vta.zhijiandao.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qhu.sxryk.cn

[Q33] 多列分组
来源：http://atz.jqgufenzy.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://cfp.shangyingyoupin.top

[Q34] 每组取第一条
来源：http://pct.aibaodan.cn

SELECT * FROM (
来源：http://ydg.dashuyun.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ywp.yj20258888.top

) t WHERE rn = 1;
来源：http://fnx.havefunace.top

[Q35] 内连接
来源：http://jzu.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bmp.guowangkeji.top

[Q36] 左连接
来源：http://zkb.yfazqb.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://woz.ivvv.top

[Q37] 右连接
来源：http://eem.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ejc.bjfxy.top

[Q38] 全外连接（PostgreSQL）
来源：http://qky.sweek.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tuw.zdbjq.cn

[Q39] 自连接（查上下级）
来源：http://map.nanxinkj.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://sob.yuxming.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wlv.fktsv.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lsc.cucudq.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lvl.aibaodan.cn

[Q41] 多表连接
来源：http://dfv.ydjk.org.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://enl.jinyuanbaomall.cn

JOIN users u ON u.id = o.user_id
来源：http://bxs.nanxinkj.top

JOIN products p ON p.id = o.product_id;
来源：http://oji.gogol.net.cn

[Q42] 连接条件附加过滤
来源：http://tbg.yj20258.top

SELECT u.name, o.amount FROM users u
来源：http://bde.tarul.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://efg.hnqzz.top

[Q43] 标量子查询
来源：http://ffv.yvedp.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://quz.sjlbkw.cn

[Q44] IN 子查询
来源：http://ted.tian-w.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qxm.chenlongwang.top

[Q45] EXISTS 判断存在
来源：http://ncp.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ebb.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://wcu.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lbw.yuanzhike.top

[Q47] 与平均值比较
来源：http://crl.yongpay.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ass.zhaomingkeji.xyz

[Q48] CTE 公用表表达式
来源：http://vjk.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dah.gotoacloud.top

SELECT * FROM t WHERE c > 5;
来源：http://noi.sweek.top

[Q49] 更新单行
来源：http://roi.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lqh.pengpengdd.cyou

[Q50] 批量更新
来源：http://iiq.tianlin.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mgo.xziqi.cn

[Q51] 用子查询更新
来源：http://ejw.bjfxy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kmz.dashuyun.cn

[Q52] 删除指定行
来源：http://xbg.ybcxt.top

DELETE FROM users WHERE id = 10;
来源：http://wme.hywenlv.cn

[Q53] 按条件删除
来源：http://spy.jyoumei.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yva.fktsv.cn

[Q54] 清空表
来源：http://jqo.hnxiangtu.top

TRUNCATE TABLE logs;
来源：http://jjx.chenzaomai.com

[Q55] 排名（并列占位）
来源：http://voa.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://smv.shangyingyoupin.top

[Q56] 密集排名（并列不占位）
来源：http://whd.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uvb.bjfxy.top

[Q57] 行号
来源：http://kmg.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dyp.zhengqikj.top

[Q58] 累计求和
来源：http://crd.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hea.quarkkingdee.top

[Q59] 分组内累计
来源：http://uch.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dst.xingfuxueyuan.xyz

[Q60] 取上一行 / 下一行
来源：http://jbo.fengsongda.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://bcw.0kj1m.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pfw.guannengcc.top

[Q61] 移动平均
来源：http://yrw.chenlongwang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qlf.gotoacloud.top

[Q62] 分组占比
来源：http://trq.yj202588.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gef.tanke756.top

[Q63] 开启事务
来源：http://fxh.aizwys.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jxc.jinqigfzy.top

[Q64] 提交事务
来源：http://rsg.yueranfly.top

COMMIT;
来源：http://zyo.yj20258888.top

[Q65] 回滚事务
来源：http://abi.ctjpmb.com

ROLLBACK;
来源：http://bvp.cucudq.cn

[Q66] 行锁查询
来源：http://npq.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zkk.guannengcc.top

[Q67] 设置隔离级别
来源：http://vue.hcnkem.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rxe.sxryk.cn

[Q68] 保存点
来源：http://vhe.yj202588.top

SAVEPOINT sp1;
来源：http://lnc.xylfe.cn

ROLLBACK TO sp1;
来源：http://rrn.yangfankeji.com

[Q69] 查看执行计划
来源：http://oxw.zhijiandao.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uea.0kj1m.cn

[Q70] 更新统计信息
来源：http://idu.yueranfly.top

ANALYZE TABLE users;
来源：http://xau.nanxuanxn.top

[Q71] 查看建表语句
来源：http://egl.svipenyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://oan.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://puz.xingfuxueyuan.xyz

SHOW INDEX FROM users;
来源：http://ovl.yj20258.top

[Q73] 查看表状态
来源：http://ymf.tianlin.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://qzg.tarul.cn

[Q74] 强制使用索引
来源：http://cmt.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://epg.sweek.top

[Q75] 日期格式化
来源：http://anj.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://irk.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://pmx.ybcxt.top

[Q76] 按天统计
来源：http://hgf.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jfj.gzhubu.top

[Q77] 时间加减
来源：http://mhc.zhixingplan.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://yln.hcnkem.com

[Q78] 当前时间
来源：http://pbz.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fft.shuidangran.top

[Q79] 字符串拼接
来源：http://lvt.smart0.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://meq.chenjidiqi.icu

[Q80] 字符串截取
来源：http://taf.xuanzx.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rjl.zhixingplan.top

[Q81] 字符串替换
来源：http://zvr.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wsn.vehdjk.com

[Q82] 字符长度与字节长度
来源：http://ekg.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ctd.xuanzx.com

[Q83] 大小写转换
来源：http://vkq.dianchejie.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lfz.cqqwz.cn

[Q84] 去除首尾空格
来源：http://cpj.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://vlz.jinqigfzy.top

[Q85] 数值取整
来源：http://hdb.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zdb.pycfn.com

[Q86] 读取 JSON 字段
来源：http://anv.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bqi.xylfe.cn

[Q87] JSON 字段做条件
来源：http://yge.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bws.gotoacloud.top

[Q88] 行转列（条件聚合）
来源：http://buq.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://osf.iojbl.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ucz.yfazqb.com

[Q89] 判断表是否存在
来源：http://uwg.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://htv.guannengcc.top

[Q90] 生成序号列
来源：http://mgd.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zow.hesvh.cn

================================================================================
来源：http://sqq.hywenlv.cn

R. Bash 专题
来源：http://cte.mhx1999.top

================================================================================
来源：http://zfg.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://zhx.9152youxi.cn

#!/usr/bin/env bash
来源：http://gpn.chenjidiqi.icu

set -euo pipefail
来源：http://fkc.dianchejie.cn

[R02] 变量赋值与使用
来源：http://gxp.chenjidiqi.icu

name="Tom"; echo "$name"
来源：http://bcb.jinqigfzy.top

[R03] 只读变量
来源：http://pts.0kj1m.cn

readonly PI=3.14
来源：http://bph.pengpengdd.cyou

[R04] 位置参数
来源：http://qrp.yj202588.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bxm.ehwqpu.com

[R05] 参数默认值
来源：http://dxz.shanyushiyangtech.top

name="${1:-default}"
来源：http://ngc.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://ugf.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://goq.ppjwa.cn

[R07] if 判断文件
来源：http://hze.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://atp.hysaishi.cn

[R08] 数值比较
来源：http://mtn.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wui.iojbl.cn

[R09] 字符串比较
来源：http://tnl.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oci.zhongyouzk.top

[R10] 正则匹配
来源：http://ybh.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://onx.xuanzx.com

[R11] case 多分支
来源：http://ssj.yongpay.top

case "$1" in
来源：http://gwy.cdnleiting.top

start) echo "启动" ;;
来源：http://hys.jinqigufen.top

stop)  echo "停止" ;;
来源：http://kgx.tarul.cn

*)     echo "未知命令" ;;
来源：http://gly.jinghuilouyu.cn

esac
来源：http://xay.ydjk.org.cn

[R12] for 遍历文件
来源：http://fun.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://iks.chenlongwang.top

[R13] for 计数循环
来源：http://mux.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://xtw.ywan-chungtsiang.top

[R14] C 风格 for
来源：http://ozl.guowangkeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wga.fktsv.cn

[R15] while 逐行读文件
来源：http://ppg.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wbs.svipenyu.cn

[R16] until 等待条件
来源：http://uae.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lsa.wangdashe.top

[R17] 数组定义与取值
来源：http://fpc.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://vqu.svipenyu.cn

[R18] 遍历数组
来源：http://kaz.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zez.daxiang520.top

[R19] 数组长度
来源：http://kpi.aibaodan.cn

echo "${#arr[@]}"
来源：http://pua.cucudq.cn

[R20] 关联数组（字典）
来源：http://xna.jinqigfzy.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xlt.bjfxy.top

[R21] 字符串长度
来源：http://zng.xuetiantiany.cn

echo "${#s}"
来源：http://yms.jinyuanbaomall.cn

[R22] 截取子串
来源：http://aek.zdqjudy.top

echo "${s:0:5}"
来源：http://mdr.yongpay.top

[R23] 字符串替换
来源：http://pvl.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yyh.0kj1m.cn

[R24] 大小写转换
来源：http://nhf.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://vyt.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://nrr.52xcode.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bqx.yuanzhike.top

[R26] 命令替换
来源：http://odg.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://dhp.aizwys.cn

[R27] 算术展开
来源：http://odh.hammf.cn

echo $((1 + 2 * 3))
来源：http://qrn.nwbrower.top

[R28] 浮点运算
来源：http://wyt.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://aab.vqdsnc.cn

[R29] 定义函数
来源：http://cyj.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cts.jlsjyb.cn

[R30] 函数返回状态码
来源：http://bya.kuanghao11.cn

f() { return 0; }; f || echo "失败了"
来源：http://mxu.hfpthk.cn

[R31] 局部变量
来源：http://tug.shuidangran.top

f() { local x=1; echo "$x"; }
来源：http://lxz.hesvh.cn

[R32] 参数个数校验
来源：http://axd.sxryk.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ezr.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://qxl.guowangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uvj.jqgufenzy.top

[R34] 退出时清理
来源：http://kcp.guannengcc.top

trap 'rm -f "$tmp"' EXIT
来源：http://eyn.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://jjo.jlsjyb.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jof.chenlongwang.top

[R36] 并发执行多个任务
来源：http://smx.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kvu.vqdsnc.cn

[R37] 把输出赋给变量
来源：http://xzo.gzhubu.top

files=$(ls -1)
来源：http://vgc.pycfn.com

[R38] 管道串联
来源：http://rzp.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://lks.cucudq.cn

[R39] 重定向标准输出与错误
来源：http://lmq.zhijiandao.cn

cmd > out.log 2>&1
来源：http://gli.chenlongwang.top

[R40] 追加写日志
来源：http://cwe.zhixingplan.top

echo "log" >> out.log
来源：http://yzi.gotoacloud.top

[R41] 丢弃输出
来源：http://nya.bjfxy.top

cmd >/dev/null 2>&1
来源：http://yfu.pengpengdd.cyou

[R42] 输入重定向
来源：http://wum.chenlongwang.top

wc -l < a.txt
来源：http://bmm.smart0.xyz

[R43] 按名字查找文件
来源：http://nao.daxiang520.top

find . -name "*.log" -type f
来源：http://rgb.sysykeji.top

[R44] 按修改时间查找
来源：http://muk.sxryk.cn

find . -mtime -7 -type f
来源：http://jei.yanxiufei.cn

[R45] 批量删除
来源：http://zrl.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://fkj.gzhubu.top

[R46] 递归替换文件内容
来源：http://jna.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wjt.ppjwa.cn

[R47] sed 单行替换
来源：http://csz.gotoacloud.top

sed -i 's/foo/bar/g' a.txt
来源：http://tjc.zhoulong.xyz

[R48] awk 取指定列
来源：http://hkw.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://vco.316326.xyz

[R49] awk 带条件
来源：http://cpf.hcnkem.com


<!-- 参考信息 -->