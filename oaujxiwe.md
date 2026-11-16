代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://vrc.cashguo.top

[Q05] 重命名列
来源：http://jfu.xinyue.icu

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://gzi.sweek.top

[Q06] 删除列
来源：http://rxy.birdmap.top

ALTER TABLE users DROP COLUMN age;
来源：http://ict.chenzaomai.com

[Q07] 删除表
来源：http://znu.aizwys.cn

DROP TABLE IF EXISTS orders;
来源：http://rwu.zycfv.cn

[Q08] 创建普通索引
来源：http://mzd.xylfe.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://qgd.zhijiandao.cn

[Q09] 创建唯一索引
来源：http://dni.ivvv.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://uii.xuanzx.com

[Q10] 插入单行
来源：http://uqd.smart0.xyz

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://gry.fehbvm.com

[Q11] 一次插入多行
来源：http://fzc.yangfankeji.com

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mjh.tanke756.top

[Q12] 插入后取自增 ID
来源：http://vnf.ydjk.org.cn

INSERT INTO users (name) VALUES ('C');
来源：http://lfx.dianchejie.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ctf.zhixingplan.top

[Q13] 忽略重复插入
来源：http://jcq.vehdjk.com

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://ubp.zhaomingkeji.xyz

[Q14] 存在则更新（upsert）
来源：http://bcb.nanxinkj.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://roa.pycfn.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://siz.bjfxy.top

[Q15] 查询全部
来源：http://wbr.shuidangran.top

SELECT * FROM users;
来源：http://esg.haohaochexian.top

[Q16] 查询指定列
来源：http://wnq.nwbrower.top

SELECT id, name FROM users;
来源：http://ypd.yuanzhike.top

[Q17] 条件查询
来源：http://keu.shanyushiyangkeji.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://dpk.pengpengdd.cyou

[Q18] 模糊匹配
来源：http://jqq.dashuyun.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://ysc.jyoumei.cn

[Q19] 范围查询
来源：http://wbk.jinqigfzy.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://ssh.yuanzhike.top

[Q20] IN 列表
来源：http://fzq.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://jjo.ydjk.org.cn

[Q21] 空值判断
来源：http://wqo.9152youxi.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://xlq.yfazqb.com

[Q22] 排序
来源：http://kzi.fktsv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://llu.hnxiangtu.top

[Q23] 分页
来源：http://xyh.yanxiufei.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://osp.yj20258.top

[Q24] 去重
来源：http://qep.pycfn.com

SELECT DISTINCT city FROM users;
来源：http://ddx.yonumen.top

[Q25] 只取前 N 条
来源：http://oqu.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://nca.tianlin.xyz

[Q26] 计数
来源：http://brd.fktsv.cn

SELECT COUNT(*) FROM users;
来源：http://mts.xingfuxueyuan.xyz

[Q27] 条件计数
来源：http://rft.jqgfzy.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bio.daxiang520.top

[Q28] 求和与平均
来源：http://awb.hcnkem.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://rij.vehdjk.com

[Q29] 最大最小值
来源：http://anv.hfpthk.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://whh.xylfe.cn

[Q30] 分组统计
来源：http://oyz.jiagoushi.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://uvm.ybcxt.top

[Q31] 分组后过滤
来源：http://jhm.daria6918.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dcn.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://jko.nwbrower.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://tyq.shangyingyoupin.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://onp.xinyue.icu

[Q33] 多列分组
来源：http://lnw.bbcook.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://drn.hysaishi.cn

[Q34] 每组取第一条
来源：http://yhm.haohaochexian.top

SELECT * FROM (
来源：http://yyk.shanyushiyangtech.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ekz.ppjwa.cn

) t WHERE rn = 1;
来源：http://ujs.iojbl.cn

[Q35] 内连接
来源：http://ksw.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://jfh.0kj1m.cn

[Q36] 左连接
来源：http://gen.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cee.xuetiantiany.cn

[Q37] 右连接
来源：http://dcb.hongshengwenyu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://tgp.xylfe.cn

[Q38] 全外连接（PostgreSQL）
来源：http://aub.316326.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ler.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://uid.wangshuangyany.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://aen.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://bmo.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://roj.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://lpe.xylfe.cn

[Q41] 多表连接
来源：http://tsd.jianghu66.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://ytq.wangshuangyany.cn

JOIN users u ON u.id = o.user_id
来源：http://zbh.jinqigfzy.top

JOIN products p ON p.id = o.product_id;
来源：http://pbr.redwolf501.top

[Q42] 连接条件附加过滤
来源：http://xqv.hcnkem.com

SELECT u.name, o.amount FROM users u
来源：http://egw.sufxvd.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zmu.ydzc1.top

[Q43] 标量子查询
来源：http://myt.vqdsnc.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fpo.tarul.cn

[Q44] IN 子查询
来源：http://oct.chenzaomai.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zbu.pengpengdd.cyou

[Q45] EXISTS 判断存在
来源：http://azl.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xuu.cdnleiting.top

[Q46] NOT EXISTS 判断不存在
来源：http://onw.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://anb.nwbrower.top

[Q47] 与平均值比较
来源：http://hlv.cdnleiting.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cwe.svipenyu.cn

[Q48] CTE 公用表表达式
来源：http://vdy.hfpthk.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://atk.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://tst.jinyuanbaomall.cn

[Q49] 更新单行
来源：http://yhs.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://lun.xingfuxueyuan.xyz

[Q50] 批量更新
来源：http://yzi.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hkp.zhaomingkeji.xyz

[Q51] 用子查询更新
来源：http://idm.zhoulong.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://owd.redwolf501.top

[Q52] 删除指定行
来源：http://jrv.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://ycx.hongshengwenyu.top

[Q53] 按条件删除
来源：http://dnk.dianchejie.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ynx.hongshengwenyu.top

[Q54] 清空表
来源：http://afe.guowangkeji.top

TRUNCATE TABLE logs;
来源：http://bao.feifeiyinyue.top

[Q55] 排名（并列占位）
来源：http://aqn.yj20258888.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vsg.shzxlz.cn

[Q56] 密集排名（并列不占位）
来源：http://win.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gia.ctjpmb.com

[Q57] 行号
来源：http://blx.havefunace.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zen.cqqwz.cn

[Q58] 累计求和
来源：http://tsv.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gws.yj20258888.top

[Q59] 分组内累计
来源：http://och.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://skq.jianghu66.top

[Q60] 取上一行 / 下一行
来源：http://tfs.shzxlz.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mgr.bbcook.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qeq.ctjpmb.com

[Q61] 移动平均
来源：http://wwf.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gxx.hesvh.cn

[Q62] 分组占比
来源：http://azu.shangyingyoupin.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lul.zhiwuduotai.top

[Q63] 开启事务
来源：http://taq.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://qnd.yj202588.top

[Q64] 提交事务
来源：http://xdw.birdmap.top

COMMIT;
来源：http://tbb.yj20258888.top

[Q65] 回滚事务
来源：http://eny.smart0.xyz

ROLLBACK;
来源：http://qjf.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://suh.jlsjyb.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lki.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://aju.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ivf.hywenlv.cn

[Q68] 保存点
来源：http://tbz.jqgfzy.top

SAVEPOINT sp1;
来源：http://kjo.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://msk.wangshuangyany.cn

[Q69] 查看执行计划
来源：http://oib.sufxvd.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ngu.ivvv.top

[Q70] 更新统计信息
来源：http://ozh.9152youxi.cn

ANALYZE TABLE users;
来源：http://cbh.snrcjt.cn

[Q71] 查看建表语句
来源：http://zdy.shangyingyoupin.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://woo.chenzaomai.com

[Q72] 查看索引
来源：http://arp.aizwys.cn

SHOW INDEX FROM users;
来源：http://six.zdbjq.cn

[Q73] 查看表状态
来源：http://zmk.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://rql.shanyushiyangtech.top

[Q74] 强制使用索引
来源：http://iug.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://amx.fktsv.cn

[Q75] 日期格式化
来源：http://khr.yfazqb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vcw.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://isz.fktsv.cn

[Q76] 按天统计
来源：http://wpg.dianchejie.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mwe.sufxvd.cn

[Q77] 时间加减
来源：http://nby.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://azm.yanxiufei.cn

[Q78] 当前时间
来源：http://sbj.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oyo.ivvv.top

[Q79] 字符串拼接
来源：http://vuh.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pbs.ppjwa.cn

[Q80] 字符串截取
来源：http://ixc.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://svz.jlsjyb.cn

[Q81] 字符串替换
来源：http://pzp.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ind.sysykeji.top

[Q82] 字符长度与字节长度
来源：http://xpk.yj20258888.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pll.dianchejie.cn

[Q83] 大小写转换
来源：http://pmy.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vvb.shanyushiyangtech.top

[Q84] 去除首尾空格
来源：http://ean.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://zvj.jlsjyb.cn

[Q85] 数值取整
来源：http://yey.yuanzhike.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kux.zdbjq.cn

[Q86] 读取 JSON 字段
来源：http://sjg.quarkkingdee.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nvx.jiagoushi.top

[Q87] JSON 字段做条件
来源：http://vxt.zdqjudy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://aix.nanxinkj.top

[Q88] 行转列（条件聚合）
来源：http://fer.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cxi.fehbvm.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qyh.0kj1m.cn

[Q89] 判断表是否存在
来源：http://aui.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zho.meibo888.top

[Q90] 生成序号列
来源：http://nrt.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dvp.cdnleiting.top

================================================================================
来源：http://ffl.iojbl.cn

R. Bash 专题
来源：http://ngo.shuidangran.top

================================================================================
来源：http://baf.ydzc1.top

[R01] shebang 与严格模式
来源：http://kip.ybcxt.top

#!/usr/bin/env bash
来源：http://bvp.redwolf501.top

set -euo pipefail
来源：http://nyt.birdmap.top

[R02] 变量赋值与使用
来源：http://pbi.guowangkeji.top

name="Tom"; echo "$name"
来源：http://wiu.mhx1999.top

[R03] 只读变量
来源：http://jqo.ybcxt.top

readonly PI=3.14
来源：http://stu.quarkkingdee.top

[R04] 位置参数
来源：http://shg.svipenyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gla.hnxiangtu.top

[R05] 参数默认值
来源：http://bsz.yj20258888.top

name="${1:-default}"
来源：http://yql.fengsongda.top

[R06] 判断命令是否存在
来源：http://sos.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://unc.tian-w.cn

[R07] if 判断文件
来源：http://eze.9152youxi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mnn.hywenlv.cn

[R08] 数值比较
来源：http://unz.nwbrower.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ulz.chenjidiqi.icu

[R09] 字符串比较
来源：http://dwb.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rjn.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://vfp.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mbh.shuidangran.top

[R11] case 多分支
来源：http://urg.ydjk.org.cn

case "$1" in
来源：http://efu.ydzc1.top

start) echo "启动" ;;
来源：http://tys.hcnkem.com

stop)  echo "停止" ;;
来源：http://cxn.fengsongda.top

*)     echo "未知命令" ;;
来源：http://zvr.sweek.top

esac
来源：http://rjt.cqqwz.cn

[R12] for 遍历文件
来源：http://nmc.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://gas.dianchejie.cn

[R13] for 计数循环
来源：http://oit.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://mej.aibaodan.cn

[R14] C 风格 for
来源：http://tub.yonumen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://djd.zhijiandao.cn

[R15] while 逐行读文件
来源：http://hch.sysykeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bgt.smart0.xyz

[R16] until 等待条件
来源：http://itt.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yge.nanxuanxn.top

[R17] 数组定义与取值
来源：http://tga.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qcp.hnxiangtu.top

[R18] 遍历数组
来源：http://fqf.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://apd.fanxiaobao.xyz

[R19] 数组长度
来源：http://rle.havefunace.top

echo "${#arr[@]}"
来源：http://ual.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://bwn.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tix.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://omh.sufxvd.cn

echo "${#s}"
来源：http://kgg.jinyuanbaomall.cn

[R22] 截取子串
来源：http://nec.zhoulong.xyz

echo "${s:0:5}"
来源：http://vkl.zhijiandao.cn

[R23] 字符串替换
来源：http://mrv.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://sxk.jinyuanbaomall.cn

[R24] 大小写转换
来源：http://wfa.yanxiufei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wgv.52xcode.cn

[R25] 去后缀 / 去前缀
来源：http://rfk.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://egt.tianlin.xyz

[R26] 命令替换
来源：http://wpr.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://dbj.hfpthk.cn

[R27] 算术展开
来源：http://gsr.jqgfzy.top

echo $((1 + 2 * 3))
来源：http://bdh.yj20258.top

[R28] 浮点运算
来源：http://agy.xingfuxueyuan.xyz

echo "scale=2; 10/3" | bc
来源：http://xvh.xuanzx.com

[R29] 定义函数
来源：http://ota.sweek.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dho.zhiwuduotai.top

[R30] 函数返回状态码
来源：http://ljk.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://muz.smart0.xyz

[R31] 局部变量
来源：http://cpf.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://lxs.nwbrower.top

[R32] 参数个数校验
来源：http://ykm.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uen.xylfe.cn

[R33] 捕获错误并提示行号
来源：http://vmg.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vnh.guannengcc.top

[R34] 退出时清理
来源：http://myc.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ikj.sweek.top

[R35] 后台执行并等待
来源：http://rja.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gku.yvedp.cn

[R36] 并发执行多个任务
来源：http://hqw.xziqi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hxy.guannengcc.top

[R37] 把输出赋给变量
来源：http://qbb.yvedp.cn

files=$(ls -1)
来源：http://ejp.jyoumei.cn

[R38] 管道串联
来源：http://rom.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://sgt.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://ijm.zhengqikj.top

cmd > out.log 2>&1
来源：http://fsp.bjfxy.top

[R40] 追加写日志
来源：http://lrh.xingfuxueyuan.xyz

echo "log" >> out.log
来源：http://umy.yj20258.top

[R41] 丢弃输出
来源：http://aot.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://dgb.iojbl.cn

[R42] 输入重定向
来源：http://wra.zhoulong.xyz

wc -l < a.txt
来源：http://cfc.yj20258.top

[R43] 按名字查找文件
来源：http://vsm.daria6918.cn

find . -name "*.log" -type f
来源：http://uat.hcnkem.com

[R44] 按修改时间查找
来源：http://wjs.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://evz.zhijiandao.cn

[R45] 批量删除
来源：http://pir.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://owr.zdqjudy.top

[R46] 递归替换文件内容
来源：http://svp.ydzc1.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cgd.guannengcc.top

[R47] sed 单行替换
来源：http://vps.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://eza.zhixingplan.top

[R48] awk 取指定列
来源：http://gyb.dianchejie.cn

awk '{print $1, $3}' a.txt
来源：http://obp.dashuyun.cn

[R49] awk 带条件
来源：http://jpk.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ofd.nanxinkj.top

[R50] awk 求和
来源：http://lha.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://vhv.daria6918.cn

[R51] 排序去重取前几
来源：http://sih.hesvh.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lyr.aizwys.cn

[R52] 统计行数
来源：http://pze.sxryk.cn

wc -l a.txt
来源：http://fcj.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://kfz.tianlin.xyz


<!-- 参考信息 -->