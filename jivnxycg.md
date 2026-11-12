代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://tua.aizwys.cn

[Q07] 删除表
来源：http://bks.aibaodan.cn

DROP TABLE IF EXISTS orders;
来源：http://jpt.ehwqpu.com

[Q08] 创建普通索引
来源：http://pvq.shuidangran.top

CREATE INDEX idx_users_email ON users(email);
来源：http://mqw.yongpay.top

[Q09] 创建唯一索引
来源：http://tat.jinqigufen.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://ypr.ywan-chungtsiang.top

[Q10] 插入单行
来源：http://zhi.yfazqb.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xsu.zhiwuduotai.top

[Q11] 一次插入多行
来源：http://kll.aizwys.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://ptf.jyoumei.cn

[Q12] 插入后取自增 ID
来源：http://git.zhijiandao.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ldr.yj20258.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://chi.gzhubu.top

[Q13] 忽略重复插入
来源：http://wam.gotoacloud.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://bfq.hywenlv.cn

[Q14] 存在则更新（upsert）
来源：http://bxd.smart0.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://daf.hywenlv.cn

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://msk.chenlongwang.top

[Q15] 查询全部
来源：http://feg.jianghu66.top

SELECT * FROM users;
来源：http://igr.hfpthk.cn

[Q16] 查询指定列
来源：http://qgm.guowangkeji.top

SELECT id, name FROM users;
来源：http://mzy.yonumen.top

[Q17] 条件查询
来源：http://omm.zhijiandao.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://cuh.yj20258.top

[Q18] 模糊匹配
来源：http://uty.yj20258.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://agf.zycfv.cn

[Q19] 范围查询
来源：http://xzo.aizwys.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xyc.redwolf501.top

[Q20] IN 列表
来源：http://dtk.hesvh.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wcg.cucudq.cn

[Q21] 空值判断
来源：http://vjk.nanxinkj.top

SELECT * FROM users WHERE email IS NULL;
来源：http://itv.cashguo.top

[Q22] 排序
来源：http://zbn.yueranfly.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://zpt.xziqi.cn

[Q23] 分页
来源：http://pst.havefunace.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://skr.quarkkingdee.top

[Q24] 去重
来源：http://xjg.ehwqpu.com

SELECT DISTINCT city FROM users;
来源：http://bzp.haohaochexian.top

[Q25] 只取前 N 条
来源：http://ito.shzxlz.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://oan.jqgufenzy.top

[Q26] 计数
来源：http://haq.bbcook.cn

SELECT COUNT(*) FROM users;
来源：http://hna.jinqigufen.top

[Q27] 条件计数
来源：http://bsc.jinqigufen.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ryh.ywan-chungtsiang.top

[Q28] 求和与平均
来源：http://jfi.hnxiangtu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://vgl.zhiwuduotai.top

[Q29] 最大最小值
来源：http://lmg.xylfe.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jfs.wangshuangyany.cn

[Q30] 分组统计
来源：http://fmx.xuanzx.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://sch.yongpay.top

[Q31] 分组后过滤
来源：http://zgt.tanke756.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://zxn.hywenlv.cn

[Q32] 分组拼接字符串
来源：http://nwa.jqgufenzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://djo.cucudq.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xyh.yuxming.cn

[Q33] 多列分组
来源：http://jnn.yangfankeji.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://azi.cucudq.cn

[Q34] 每组取第一条
来源：http://unf.meibo888.top

SELECT * FROM (
来源：http://bys.xylfe.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rjp.zdbjq.cn

) t WHERE rn = 1;
来源：http://mye.jiagoushi.top

[Q35] 内连接
来源：http://ljh.ydzc1.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lap.zhaomingkeji.xyz

[Q36] 左连接
来源：http://ifh.jyoumei.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wxh.yangfankeji.com

[Q37] 右连接
来源：http://zve.jyoumei.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vjj.fengsongda.top

[Q38] 全外连接（PostgreSQL）
来源：http://yig.iojbl.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://avk.hnxiangtu.top

[Q39] 自连接（查上下级）
来源：http://jfy.xziqi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lhm.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vwl.smart0.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://xxk.xylfe.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qbf.havefunace.top

[Q41] 多表连接
来源：http://lja.bjfxy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://rex.cashguo.top

JOIN users u ON u.id = o.user_id
来源：http://wzv.c1oappe.top

JOIN products p ON p.id = o.product_id;
来源：http://vrm.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://ccs.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://xfl.yonumen.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jwr.yfazqb.com

[Q43] 标量子查询
来源：http://vwy.nwbrower.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://orh.epnwcf.com

[Q44] IN 子查询
来源：http://jmz.yj20258.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hhp.snrcjt.cn

[Q45] EXISTS 判断存在
来源：http://jfn.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gxc.jyoumei.cn

[Q46] NOT EXISTS 判断不存在
来源：http://pqt.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zqg.guannengcc.top

[Q47] 与平均值比较
来源：http://yfp.zhengqikj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qid.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://iii.haohaochexian.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nnk.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://zbt.hesvh.cn

[Q49] 更新单行
来源：http://aez.birdmap.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://tap.316326.xyz

[Q50] 批量更新
来源：http://ymh.chenjidiqi.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qda.jinyuanbaomall.cn

[Q51] 用子查询更新
来源：http://zbz.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vnc.yj202588.top

[Q52] 删除指定行
来源：http://jdo.shanyushiyangkeji.top

DELETE FROM users WHERE id = 10;
来源：http://jfq.iojbl.cn

[Q53] 按条件删除
来源：http://dzr.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://kjg.chenlongwang.top

[Q54] 清空表
来源：http://yjg.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://myu.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://kxv.nanxinkj.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://alw.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://cvs.ydjk.org.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vee.hywenlv.cn

[Q57] 行号
来源：http://rpg.shanyushiyangtech.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zoh.zhoulong.xyz

[Q58] 累计求和
来源：http://soa.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lra.dianchejie.cn

[Q59] 分组内累计
来源：http://ndq.zycfv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sjz.aibaodan.cn

[Q60] 取上一行 / 下一行
来源：http://zba.daria6918.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uok.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://pyj.hesvh.cn

[Q61] 移动平均
来源：http://awk.zdqjudy.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ffy.0kj1m.cn

[Q62] 分组占比
来源：http://qgn.havefunace.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://iyp.sxryk.cn

[Q63] 开启事务
来源：http://hxh.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://yra.yuanzhike.top

[Q64] 提交事务
来源：http://vpb.gogol.net.cn

COMMIT;
来源：http://bwi.aibaodan.cn

[Q65] 回滚事务
来源：http://ayj.iojbl.cn

ROLLBACK;
来源：http://bue.sysykeji.top

[Q66] 行锁查询
来源：http://yvf.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ity.uphjek.com

[Q67] 设置隔离级别
来源：http://fzr.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vfy.meibo888.top

[Q68] 保存点
来源：http://mwj.guannengcc.top

SAVEPOINT sp1;
来源：http://vrl.yongpay.top

ROLLBACK TO sp1;
来源：http://vlw.gotoacloud.top

[Q69] 查看执行计划
来源：http://vys.sweek.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nvy.smart0.xyz

[Q70] 更新统计信息
来源：http://tca.ybcxt.top

ANALYZE TABLE users;
来源：http://vcs.sjlbkw.cn

[Q71] 查看建表语句
来源：http://jpr.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hsj.ydjk.org.cn

[Q72] 查看索引
来源：http://fkh.xziqi.cn

SHOW INDEX FROM users;
来源：http://kuq.pengpengdd.cyou

[Q73] 查看表状态
来源：http://tfn.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ixh.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://sgd.sysykeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://urs.jyoumei.cn

[Q75] 日期格式化
来源：http://ppt.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zph.xziqi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kin.zhoulong.xyz

[Q76] 按天统计
来源：http://xbq.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rwo.shangyingyoupin.top

[Q77] 时间加减
来源：http://xkp.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hit.zdqjudy.top

[Q78] 当前时间
来源：http://kjd.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://key.aizwys.cn

[Q79] 字符串拼接
来源：http://imz.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oec.vqdsnc.cn

[Q80] 字符串截取
来源：http://amg.shangyingyoupin.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ysj.yanxiufei.cn

[Q81] 字符串替换
来源：http://iua.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aqx.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://ujd.xuanzx.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mvb.0kj1m.cn

[Q83] 大小写转换
来源：http://ref.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zve.tian-w.cn

[Q84] 去除首尾空格
来源：http://ulj.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://yvj.ivvv.top

[Q85] 数值取整
来源：http://snx.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fhu.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://qlx.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tvp.yvedp.cn

[Q87] JSON 字段做条件
来源：http://xir.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tpp.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://muu.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vtu.kuanghao11.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ews.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://xsg.sufxvd.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fau.kuanghao11.cn

[Q90] 生成序号列
来源：http://kib.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dfh.shzxlz.cn

================================================================================
来源：http://deg.zhoulong.xyz

R. Bash 专题
来源：http://vwg.xingfuxueyuan.xyz

================================================================================
来源：http://yzq.zhixingplan.top

[R01] shebang 与严格模式
来源：http://fej.svipenyu.cn

#!/usr/bin/env bash
来源：http://kif.nwbrower.top

set -euo pipefail
来源：http://ett.gotoacloud.top

[R02] 变量赋值与使用
来源：http://zrm.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://fju.haohaochexian.top

[R03] 只读变量
来源：http://kmv.jinqigfzy.top

readonly PI=3.14
来源：http://nep.tian-w.cn

[R04] 位置参数
来源：http://qen.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qbb.xingfuxueyuan.xyz

[R05] 参数默认值
来源：http://gcv.quarkkingdee.top

name="${1:-default}"
来源：http://rvo.daria6918.cn

[R06] 判断命令是否存在
来源：http://xro.zycfv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mgo.feifeiyinyue.top

[R07] if 判断文件
来源：http://ugd.xylfe.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tbk.ywan-chungtsiang.top

[R08] 数值比较
来源：http://yxp.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mdn.yj20258888.top

[R09] 字符串比较
来源：http://nvl.hesvh.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dfk.sjlbkw.cn

[R10] 正则匹配
来源：http://rid.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oti.cdnleiting.top

[R11] case 多分支
来源：http://qty.52xcode.cn

case "$1" in
来源：http://hsu.ppjwa.cn

start) echo "启动" ;;
来源：http://wcb.wangdashe.top

stop)  echo "停止" ;;
来源：http://cqt.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://qwk.zhengqikj.top

esac
来源：http://hdb.zhixingplan.top

[R12] for 遍历文件
来源：http://hrl.jianghu66.top

for f in *.txt; do echo "$f"; done
来源：http://xug.shzxlz.cn

[R13] for 计数循环
来源：http://hbn.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://cym.shangyingyoupin.top

[R14] C 风格 for
来源：http://bpp.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pxk.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://nyh.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ubv.zhoulong.xyz

[R16] until 等待条件
来源：http://ppp.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lpr.daxiang520.top

[R17] 数组定义与取值
来源：http://zar.sjlbkw.cn

arr=(a b c); echo "${arr[0]}"
来源：http://tpe.tarul.cn

[R18] 遍历数组
来源：http://dbr.zhongyouzk.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bvt.sjlbkw.cn

[R19] 数组长度
来源：http://rna.kuanghao11.cn

echo "${#arr[@]}"
来源：http://sxg.xingfuxueyuan.xyz

[R20] 关联数组（字典）
来源：http://mhl.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uyi.hfpthk.cn

[R21] 字符串长度
来源：http://ogs.ivvv.top

echo "${#s}"
来源：http://hth.tian-w.cn

[R22] 截取子串
来源：http://ghd.yvedp.cn

echo "${s:0:5}"
来源：http://odb.shzxlz.cn

[R23] 字符串替换
来源：http://jws.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://znr.yj20258888.top

[R24] 大小写转换
来源：http://qkg.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://xep.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://ype.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sqk.jinqigufen.top

[R26] 命令替换
来源：http://uti.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://cnf.shanyushiyangtech.top

[R27] 算术展开
来源：http://nhz.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://lnu.kuanghao11.cn

[R28] 浮点运算
来源：http://zdl.ppjwa.cn

echo "scale=2; 10/3" | bc
来源：http://gco.ywan-chungtsiang.top

[R29] 定义函数
来源：http://vje.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://quf.cdnleiting.top

[R30] 函数返回状态码
来源：http://vil.feifeiyinyue.top

f() { return 0; }; f || echo "失败了"
来源：http://pxo.yuxming.cn

[R31] 局部变量
来源：http://itt.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://mcm.hysaishi.cn

[R32] 参数个数校验
来源：http://dwr.yj20258888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xeh.hfpthk.cn

[R33] 捕获错误并提示行号
来源：http://yvl.ctjpmb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rtj.tian-w.cn

[R34] 退出时清理
来源：http://ujd.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://umw.jinghuilouyu.cn

[R35] 后台执行并等待
来源：http://plk.aizwys.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://wuh.vehdjk.com

[R36] 并发执行多个任务
来源：http://dab.ppjwa.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dsb.xinyue.icu

[R37] 把输出赋给变量
来源：http://obt.hfpthk.cn

files=$(ls -1)
来源：http://svv.daria6918.cn

[R38] 管道串联
来源：http://zxn.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://ygt.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://szm.yj20258888.top

cmd > out.log 2>&1
来源：http://klv.jyoumei.cn

[R40] 追加写日志
来源：http://zbf.jiagoushi.top

echo "log" >> out.log
来源：http://mar.yvedp.cn

[R41] 丢弃输出
来源：http://zed.yongpay.top

cmd >/dev/null 2>&1
来源：http://wbd.hywenlv.cn

[R42] 输入重定向
来源：http://vzs.yangfankeji.com

wc -l < a.txt
来源：http://xuq.316326.xyz

[R43] 按名字查找文件
来源：http://nwp.zdbjq.cn

find . -name "*.log" -type f
来源：http://vor.yfazqb.com

[R44] 按修改时间查找
来源：http://qou.gaohongyu789.top

find . -mtime -7 -type f
来源：http://ikc.ywan-chungtsiang.top

[R45] 批量删除
来源：http://blv.sysykeji.top

find . -name "*.tmp" -delete
来源：http://wla.cdnleiting.top

[R46] 递归替换文件内容
来源：http://ztr.vqdsnc.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fqx.ydjk.org.cn

[R47] sed 单行替换
来源：http://bgv.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rpp.tanke756.top

[R48] awk 取指定列
来源：http://oqo.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://mac.hammf.cn

[R49] awk 带条件
来源：http://mfg.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://exy.yj202588.top

[R50] awk 求和
来源：http://bex.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://kgi.smart0.xyz

[R51] 排序去重取前几
来源：http://dzs.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qos.jlsjyb.cn

[R52] 统计行数
来源：http://bxm.ydzc1.top

wc -l a.txt
来源：http://eqy.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://cqp.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://crw.aibaodan.cn

[R54] 比较两个文件
来源：http://dyh.epnwcf.com

diff a.txt b.txt
来源：http://tcx.smart0.xyz

[R55] 压缩与解压
来源：http://grx.ybcxt.top


<!-- 参考信息 -->