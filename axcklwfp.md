代发 wailian999

);
来源：http://dxl.ppjwa.cn

[Q03] 增加列
来源：http://gsh.tanke756.top

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://rxv.nwbrower.top

[Q04] 修改列类型
来源：http://pdr.jqgfzy.top

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://rxc.hnqzz.top

[Q05] 重命名列
来源：http://jbt.sufxvd.cn

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://bwj.jianghu66.top

[Q06] 删除列
来源：http://eox.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://tjo.xuetiantiany.cn

[Q07] 删除表
来源：http://wzu.cdnleiting.top

DROP TABLE IF EXISTS orders;
来源：http://zxz.cqqwz.cn

[Q08] 创建普通索引
来源：http://sie.svipenyu.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://njq.yangfankeji.com

[Q09] 创建唯一索引
来源：http://pqe.yuxming.cn

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://yzo.ybcxt.top

[Q10] 插入单行
来源：http://ixv.bbcook.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://xed.zhongyouzk.top

[Q11] 一次插入多行
来源：http://kyu.fanxiaobao.xyz

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wjf.hnqzz.top

[Q12] 插入后取自增 ID
来源：http://zot.jinqigufen.top

INSERT INTO users (name) VALUES ('C');
来源：http://cdg.ydzc1.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://nku.nanxinkj.top

[Q13] 忽略重复插入
来源：http://xmw.chenlongwang.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://zqy.cashguo.top

[Q14] 存在则更新（upsert）
来源：http://ccc.fktsv.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://htu.jiagoushi.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://fnl.jqgufenzy.top

[Q15] 查询全部
来源：http://liv.epnwcf.com

SELECT * FROM users;
来源：http://ygg.jinqigfzy.top

[Q16] 查询指定列
来源：http://uks.chenjidiqi.icu

SELECT id, name FROM users;
来源：http://mxx.zhiwuduotai.top

[Q17] 条件查询
来源：http://hot.uphjek.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://zss.ywan-chungtsiang.top

[Q18] 模糊匹配
来源：http://kod.cheryme.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://eqi.jiagoushi.top

[Q19] 范围查询
来源：http://lgr.cdnleiting.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://klg.zhiwuduotai.top

[Q20] IN 列表
来源：http://buc.ydjk.org.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://uyn.hfpthk.cn

[Q21] 空值判断
来源：http://xhd.jinyuanbaomall.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://vwu.jqgfzy.top

[Q22] 排序
来源：http://ajy.jinqigfzy.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://qiq.jinyuanbaomall.cn

[Q23] 分页
来源：http://tly.jinghuilouyu.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vly.vehdjk.com

[Q24] 去重
来源：http://yzz.sjlbkw.cn

SELECT DISTINCT city FROM users;
来源：http://gyu.svipenyu.cn

[Q25] 只取前 N 条
来源：http://bkb.chenjidiqi.icu

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://kbd.sxryk.cn

[Q26] 计数
来源：http://rdf.9152youxi.cn

SELECT COUNT(*) FROM users;
来源：http://xcd.gaohongyu789.top

[Q27] 条件计数
来源：http://okb.chenlongwang.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://stm.wangdashe.top

[Q28] 求和与平均
来源：http://fet.daria6918.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://pmt.smart0.xyz

[Q29] 最大最小值
来源：http://mmx.nwbrower.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://jus.jiagoushi.top

[Q30] 分组统计
来源：http://cky.gaohongyu789.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://nnp.xziqi.cn

[Q31] 分组后过滤
来源：http://vup.kuanghao11.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://uqb.yj202588.top

[Q32] 分组拼接字符串
来源：http://zaj.hnqzz.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://vwm.yvedp.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://tvu.fzhhl.top

[Q33] 多列分组
来源：http://wnf.cashguo.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://fan.cashguo.top

[Q34] 每组取第一条
来源：http://cqj.zdqjudy.top

SELECT * FROM (
来源：http://azf.zhixingplan.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://igg.yvedp.cn

) t WHERE rn = 1;
来源：http://ntg.hywenlv.cn

[Q35] 内连接
来源：http://yrb.mhx1999.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://fpm.jqgfzy.top

[Q36] 左连接
来源：http://mmc.nanxinkj.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://cbo.shangyingyoupin.top

[Q37] 右连接
来源：http://fwj.yongpay.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://kly.haohaochexian.top

[Q38] 全外连接（PostgreSQL）
来源：http://tpj.daxiang520.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ysv.fanxiaobao.xyz

[Q39] 自连接（查上下级）
来源：http://puh.chenjidiqi.icu

SELECT e.name, m.name AS manager FROM employees e
来源：http://icy.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hnb.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mho.c1oappe.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://vbh.quarkkingdee.top

[Q41] 多表连接
来源：http://fsb.jinqigfzy.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://wmr.ydjk.org.cn

JOIN users u ON u.id = o.user_id
来源：http://bhk.gaohongyu789.top

JOIN products p ON p.id = o.product_id;
来源：http://vqu.9152youxi.cn

[Q42] 连接条件附加过滤
来源：http://wxs.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://gjt.yanxiufei.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mgb.cashguo.top

[Q43] 标量子查询
来源：http://lfq.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hvj.yj20258.top

[Q44] IN 子查询
来源：http://hqh.birdmap.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://upm.andypj.xyz

[Q45] EXISTS 判断存在
来源：http://fbv.bjfxy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gwh.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://amf.ehwqpu.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://imh.tanke756.top

[Q47] 与平均值比较
来源：http://vwk.xingfuxueyuan.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ryx.hnxiangtu.top

[Q48] CTE 公用表表达式
来源：http://vyp.iojbl.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://swv.shangyingyoupin.top

SELECT * FROM t WHERE c > 5;
来源：http://wqj.jqgfzy.top

[Q49] 更新单行
来源：http://hrf.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://laz.zhixingplan.top

[Q50] 批量更新
来源：http://auy.xuetiantiany.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qto.yuxming.cn

[Q51] 用子查询更新
来源：http://cir.hywenlv.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vzp.vqdsnc.cn

[Q52] 删除指定行
来源：http://qwq.ydjk.org.cn

DELETE FROM users WHERE id = 10;
来源：http://qff.52xcode.cn

[Q53] 按条件删除
来源：http://quo.cdnleiting.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ujx.gaohongyu789.top

[Q54] 清空表
来源：http://qzs.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://mcj.zhiwuduotai.top

[Q55] 排名（并列占位）
来源：http://xqr.dashuyun.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ltj.yuanzhike.top

[Q56] 密集排名（并列不占位）
来源：http://cyj.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ero.sysykeji.top

[Q57] 行号
来源：http://cfj.hongshengwenyu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sgo.fanxiaobao.xyz

[Q58] 累计求和
来源：http://vbk.fehbvm.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xgu.gogol.net.cn

[Q59] 分组内累计
来源：http://ghr.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://odk.epnwcf.com

[Q60] 取上一行 / 下一行
来源：http://joh.shanyushiyangkeji.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wrx.bjfxy.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ptq.tian-w.cn

[Q61] 移动平均
来源：http://qma.hammf.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ban.ydzc1.top

[Q62] 分组占比
来源：http://akk.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lfm.sjlbkw.cn

[Q63] 开启事务
来源：http://txh.hnqzz.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fyo.pengpengdd.cyou

[Q64] 提交事务
来源：http://ptv.zhijiandao.cn

COMMIT;
来源：http://hbl.wangshuangyany.cn

[Q65] 回滚事务
来源：http://vwl.hammf.cn

ROLLBACK;
来源：http://yyi.tanke756.top

[Q66] 行锁查询
来源：http://gra.pengpengdd.cyou

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vor.hammf.cn

[Q67] 设置隔离级别
来源：http://qox.jinqigufen.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sge.tanke756.top

[Q68] 保存点
来源：http://nyz.snrcjt.cn

SAVEPOINT sp1;
来源：http://skj.yueranfly.top

ROLLBACK TO sp1;
来源：http://wiq.fzhhl.top

[Q69] 查看执行计划
来源：http://hii.jianghu66.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ymg.hnxiangtu.top

[Q70] 更新统计信息
来源：http://hgz.yonumen.top

ANALYZE TABLE users;
来源：http://gwz.yonumen.top

[Q71] 查看建表语句
来源：http://hvd.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://btz.cqqwz.cn

[Q72] 查看索引
来源：http://rfq.ppjwa.cn

SHOW INDEX FROM users;
来源：http://rqv.hongshengwenyu.top

[Q73] 查看表状态
来源：http://xht.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nrg.jianghu66.top

[Q74] 强制使用索引
来源：http://pet.tanke756.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bmw.zhongyouzk.top

[Q75] 日期格式化
来源：http://bow.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gkp.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tjy.yangfankeji.com

[Q76] 按天统计
来源：http://elf.birdmap.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gff.jinghuilouyu.cn

[Q77] 时间加减
来源：http://ryo.jyoumei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://aqm.gotoacloud.top

[Q78] 当前时间
来源：http://zzy.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yfv.ywan-chungtsiang.top

[Q79] 字符串拼接
来源：http://tvd.iojbl.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://stl.yueranfly.top

[Q80] 字符串截取
来源：http://knh.jyoumei.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qts.fehbvm.com

[Q81] 字符串替换
来源：http://qgi.52xcode.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fdd.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://abb.cucudq.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oll.ehwqpu.com

[Q83] 大小写转换
来源：http://zjj.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bkp.meibo888.top

[Q84] 去除首尾空格
来源：http://bfn.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://gdo.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://gty.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ltl.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://kux.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ooc.jyoumei.cn

[Q87] JSON 字段做条件
来源：http://vbx.hysaishi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://utn.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://owc.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yyw.birdmap.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uvy.daria6918.cn

[Q89] 判断表是否存在
来源：http://efr.ehwqpu.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://lqs.havefunace.top

[Q90] 生成序号列
来源：http://nob.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwm.daria6918.cn

================================================================================
来源：http://hig.zdqjudy.top

R. Bash 专题
来源：http://icr.aibaodan.cn

================================================================================
来源：http://xny.shuidangran.top

[R01] shebang 与严格模式
来源：http://lgl.ywan-chungtsiang.top

#!/usr/bin/env bash
来源：http://xrl.vqdsnc.cn

set -euo pipefail
来源：http://bdl.0kj1m.cn

[R02] 变量赋值与使用
来源：http://ffj.cdnleiting.top

name="Tom"; echo "$name"
来源：http://hko.xuetiantiany.cn

[R03] 只读变量
来源：http://kdy.bjfxy.top

readonly PI=3.14
来源：http://rkb.hcnkem.com

[R04] 位置参数
来源：http://afd.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bcu.gogol.net.cn

[R05] 参数默认值
来源：http://hzq.hongshengwenyu.top

name="${1:-default}"
来源：http://pys.c1oappe.top

[R06] 判断命令是否存在
来源：http://vnx.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vfb.yvedp.cn

[R07] if 判断文件
来源：http://ihn.tian-w.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kkw.smart0.xyz

[R08] 数值比较
来源：http://ztx.0kj1m.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ibm.hnxiangtu.top

[R09] 字符串比较
来源：http://bsw.yuanzhike.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hpt.pengpengdd.cyou

[R10] 正则匹配
来源：http://cyq.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hxa.daria6918.cn

[R11] case 多分支
来源：http://qcb.hnxiangtu.top

case "$1" in
来源：http://urq.yonumen.top

start) echo "启动" ;;
来源：http://kys.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://zeu.hammf.cn

*)     echo "未知命令" ;;
来源：http://zqb.xuetiantiany.cn

esac
来源：http://yle.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://hrw.zdqjudy.top

for f in *.txt; do echo "$f"; done
来源：http://rpk.tianlin.xyz

[R13] for 计数循环
来源：http://lht.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://smg.zhijiandao.cn

[R14] C 风格 for
来源：http://xer.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dsk.yueranfly.top

[R15] while 逐行读文件
来源：http://udd.iojbl.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ekn.jlsjyb.cn

[R16] until 等待条件
来源：http://ivt.snrcjt.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ytb.yj202588.top

[R17] 数组定义与取值
来源：http://pba.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fhb.zycfv.cn

[R18] 遍历数组
来源：http://uio.jlsjyb.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ukm.haohaochexian.top

[R19] 数组长度
来源：http://bcd.jinqigufen.top

echo "${#arr[@]}"
来源：http://dod.guowangkeji.top

[R20] 关联数组（字典）
来源：http://dkr.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cny.sysykeji.top

[R21] 字符串长度
来源：http://cyf.xylfe.cn

echo "${#s}"
来源：http://axs.ybcxt.top

[R22] 截取子串
来源：http://bej.zdbjq.cn

echo "${s:0:5}"
来源：http://lso.ydjk.org.cn

[R23] 字符串替换
来源：http://tkl.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mez.hnxiangtu.top

[R24] 大小写转换
来源：http://ywx.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://seu.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://dub.guannengcc.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://sxm.iojbl.cn

[R26] 命令替换
来源：http://zgt.ctjpmb.com

now=$(date +%F); echo "$now"
来源：http://dcn.epnwcf.com

[R27] 算术展开
来源：http://dla.cqqwz.cn

echo $((1 + 2 * 3))
来源：http://vis.fehbvm.com

[R28] 浮点运算
来源：http://ixv.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://pwr.shzxlz.cn

[R29] 定义函数
来源：http://jss.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tpw.daxiang520.top

[R30] 函数返回状态码
来源：http://msp.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://zpd.cheryme.top

[R31] 局部变量
来源：http://fre.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://ser.jinqigfzy.top

[R32] 参数个数校验
来源：http://tww.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bdh.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://jih.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ajx.snrcjt.cn

[R34] 退出时清理
来源：http://xyx.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://fns.ydzc1.top

[R35] 后台执行并等待
来源：http://jzx.birdmap.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tax.havefunace.top

[R36] 并发执行多个任务
来源：http://oub.jiagoushi.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://iaw.jinqigufen.top

[R37] 把输出赋给变量
来源：http://ilh.birdmap.top

files=$(ls -1)
来源：http://xys.316326.xyz

[R38] 管道串联
来源：http://jzy.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://del.havefunace.top

[R39] 重定向标准输出与错误
来源：http://sbc.feifeiyinyue.top

cmd > out.log 2>&1
来源：http://jkr.wangdashe.top

[R40] 追加写日志
来源：http://icu.shangyingyoupin.top

echo "log" >> out.log
来源：http://zxh.0kj1m.cn

[R41] 丢弃输出
来源：http://tyw.nwbrower.top

cmd >/dev/null 2>&1
来源：http://glb.zhongyouzk.top

[R42] 输入重定向
来源：http://suu.iojbl.cn

wc -l < a.txt
来源：http://vvf.wangdashe.top

[R43] 按名字查找文件
来源：http://ykl.shzxlz.cn

find . -name "*.log" -type f
来源：http://exb.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://lzg.yvedp.cn

find . -mtime -7 -type f
来源：http://awu.snrcjt.cn

[R45] 批量删除
来源：http://zek.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://cok.9152youxi.cn

[R46] 递归替换文件内容
来源：http://ovo.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://djg.ppjwa.cn

[R47] sed 单行替换
来源：http://eub.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://tyh.havefunace.top

[R48] awk 取指定列
来源：http://pnf.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://lyt.hcnkem.com

[R49] awk 带条件
来源：http://qto.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aff.daxiang520.top

[R50] awk 求和
来源：http://ick.redwolf501.top

awk '{s += $2} END {print s}' a.txt
来源：http://wfs.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://aih.feifeiyinyue.top


<!-- 参考信息 -->