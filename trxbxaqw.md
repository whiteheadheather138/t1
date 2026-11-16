代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://quz.316326.xyz

[Q09] 创建唯一索引
来源：http://eev.yj20258.top

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://efg.guannengcc.top

[Q10] 插入单行
来源：http://wae.jinyuanbaomall.cn

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://dot.nanxinkj.top

[Q11] 一次插入多行
来源：http://kwl.mhx1999.top

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://gma.birdmap.top

[Q12] 插入后取自增 ID
来源：http://hqo.sjlbkw.cn

INSERT INTO users (name) VALUES ('C');
来源：http://ggs.aibaodan.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uhm.cdnleiting.top

[Q13] 忽略重复插入
来源：http://kex.yj20258888.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://vjq.c1oappe.top

[Q14] 存在则更新（upsert）
来源：http://gpu.316326.xyz

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://cpk.tanke756.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://pff.cucudq.cn

[Q15] 查询全部
来源：http://jqu.xuetiantiany.cn

SELECT * FROM users;
来源：http://srx.gotoacloud.top

[Q16] 查询指定列
来源：http://lcv.xuanzx.com

SELECT id, name FROM users;
来源：http://nfq.ydjk.org.cn

[Q17] 条件查询
来源：http://niq.redwolf501.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://nxr.sjlbkw.cn

[Q18] 模糊匹配
来源：http://pkk.hnqzz.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qqq.hnxiangtu.top

[Q19] 范围查询
来源：http://wqd.hysaishi.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://cog.jinqigufen.top

[Q20] IN 列表
来源：http://iae.xylfe.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://lzr.dianchejie.cn

[Q21] 空值判断
来源：http://vws.yj20258888.top

SELECT * FROM users WHERE email IS NULL;
来源：http://qvy.hysaishi.cn

[Q22] 排序
来源：http://zsw.hywenlv.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://eqm.yfazqb.com

[Q23] 分页
来源：http://igy.tarul.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vck.ppjwa.cn

[Q24] 去重
来源：http://twg.zycfv.cn

SELECT DISTINCT city FROM users;
来源：http://qum.jqgfzy.top

[Q25] 只取前 N 条
来源：http://dex.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qtk.ctjpmb.com

[Q26] 计数
来源：http://aii.yvedp.cn

SELECT COUNT(*) FROM users;
来源：http://ojx.sysykeji.top

[Q27] 条件计数
来源：http://oyv.hywenlv.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wpy.zhoulong.xyz

[Q28] 求和与平均
来源：http://mgg.gotoacloud.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fli.jianghu66.top

[Q29] 最大最小值
来源：http://olm.shzxlz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://nwm.sweek.top

[Q30] 分组统计
来源：http://qnb.yangfankeji.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://lpf.shzxlz.cn

[Q31] 分组后过滤
来源：http://rcz.guowangkeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ovk.wangdashe.top

[Q32] 分组拼接字符串
来源：http://bes.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://zfh.fehbvm.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://xqc.ydjk.org.cn

[Q33] 多列分组
来源：http://ocz.cdnleiting.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://iae.hcnkem.com

[Q34] 每组取第一条
来源：http://fec.zdbjq.cn

SELECT * FROM (
来源：http://fry.iojbl.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://riy.guowangkeji.top

) t WHERE rn = 1;
来源：http://iua.nanxinkj.top

[Q35] 内连接
来源：http://ymq.wangdashe.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hlj.zycfv.cn

[Q36] 左连接
来源：http://dtt.ivvv.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mst.mhx1999.top

[Q37] 右连接
来源：http://ois.guannengcc.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vxq.mhx1999.top

[Q38] 全外连接（PostgreSQL）
来源：http://dgb.jqgfzy.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ksq.hesvh.cn

[Q39] 自连接（查上下级）
来源：http://ibm.gotoacloud.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tbq.hammf.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://til.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cbz.cashguo.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://bsg.vehdjk.com

[Q41] 多表连接
来源：http://uwb.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://gcg.bjfxy.top

JOIN users u ON u.id = o.user_id
来源：http://emn.9152youxi.cn

JOIN products p ON p.id = o.product_id;
来源：http://clh.zhongyouzk.top

[Q42] 连接条件附加过滤
来源：http://fhk.sysykeji.top

SELECT u.name, o.amount FROM users u
来源：http://ckq.fehbvm.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://vuv.c1oappe.top

[Q43] 标量子查询
来源：http://mwq.ybcxt.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://lti.sysykeji.top

[Q44] IN 子查询
来源：http://zhu.cheryme.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lss.hammf.cn

[Q45] EXISTS 判断存在
来源：http://mrn.cashguo.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wtd.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://uqc.shanyushiyangtech.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cpx.mhx1999.top

[Q47] 与平均值比较
来源：http://gza.fktsv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vhi.ydjk.org.cn

[Q48] CTE 公用表表达式
来源：http://tia.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cqb.cdnleiting.top

SELECT * FROM t WHERE c > 5;
来源：http://nlj.dashuyun.cn

[Q49] 更新单行
来源：http://imi.hongshengwenyu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nij.zdqjudy.top

[Q50] 批量更新
来源：http://fkm.fktsv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vev.ydjk.org.cn

[Q51] 用子查询更新
来源：http://ret.yj20258888.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cbm.dianchejie.cn

[Q52] 删除指定行
来源：http://yfc.52xcode.cn

DELETE FROM users WHERE id = 10;
来源：http://vjc.daria6918.cn

[Q53] 按条件删除
来源：http://rlq.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ubx.redwolf501.top

[Q54] 清空表
来源：http://ink.zhengqikj.top

TRUNCATE TABLE logs;
来源：http://obw.hcnkem.com

[Q55] 排名（并列占位）
来源：http://vpn.wangshuangyany.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tfr.cdnleiting.top

[Q56] 密集排名（并列不占位）
来源：http://yyb.hnqzz.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gxx.redwolf501.top

[Q57] 行号
来源：http://ctd.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xzh.yonumen.top

[Q58] 累计求和
来源：http://gjh.zdbjq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://azz.nanxinkj.top

[Q59] 分组内累计
来源：http://nge.9152youxi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://tgi.gotoacloud.top

[Q60] 取上一行 / 下一行
来源：http://ldr.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ihq.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cqs.zhongyouzk.top

[Q61] 移动平均
来源：http://bzk.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pel.ctjpmb.com

[Q62] 分组占比
来源：http://ski.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://unh.xylfe.cn

[Q63] 开启事务
来源：http://vhg.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gre.yonumen.top

[Q64] 提交事务
来源：http://bng.cucudq.cn

COMMIT;
来源：http://ehj.yueranfly.top

[Q65] 回滚事务
来源：http://nwr.jinyuanbaomall.cn

ROLLBACK;
来源：http://wqf.zycfv.cn

[Q66] 行锁查询
来源：http://dzr.pengpengdd.cyou

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dtk.sufxvd.cn

[Q67] 设置隔离级别
来源：http://yma.sufxvd.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fjd.zhiwuduotai.top

[Q68] 保存点
来源：http://eac.hywenlv.cn

SAVEPOINT sp1;
来源：http://cyd.smart0.xyz

ROLLBACK TO sp1;
来源：http://rdz.mhx1999.top

[Q69] 查看执行计划
来源：http://aru.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lwk.wangshuangyany.cn

[Q70] 更新统计信息
来源：http://xrw.dashuyun.cn

ANALYZE TABLE users;
来源：http://kfe.316326.xyz

[Q71] 查看建表语句
来源：http://hxu.yj20258888.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qjj.yuanzhike.top

[Q72] 查看索引
来源：http://jvz.ybcxt.top

SHOW INDEX FROM users;
来源：http://srs.0kj1m.cn

[Q73] 查看表状态
来源：http://mar.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pqu.xuanzx.com

[Q74] 强制使用索引
来源：http://voi.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://uch.gzhubu.top

[Q75] 日期格式化
来源：http://zks.chenjidiqi.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dux.sufxvd.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zbt.yangfankeji.com

[Q76] 按天统计
来源：http://wvg.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mek.hesvh.cn

[Q77] 时间加减
来源：http://zjg.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wxt.wangshuangyany.cn

[Q78] 当前时间
来源：http://ggj.xziqi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uwm.aizwys.cn

[Q79] 字符串拼接
来源：http://mnq.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://udu.kuanghao11.cn

[Q80] 字符串截取
来源：http://qzj.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cay.hysaishi.cn

[Q81] 字符串替换
来源：http://ctc.fktsv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://whf.chenzaomai.com

[Q82] 字符长度与字节长度
来源：http://rqp.cqqwz.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ydw.gogol.net.cn

[Q83] 大小写转换
来源：http://pqm.yanxiufei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dri.vqdsnc.cn

[Q84] 去除首尾空格
来源：http://art.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://keb.fzhhl.top

[Q85] 数值取整
来源：http://sbu.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jwh.hammf.cn

[Q86] 读取 JSON 字段
来源：http://cmu.zdqjudy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://soi.gaohongyu789.top

[Q87] JSON 字段做条件
来源：http://irm.bbcook.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxu.pengpengdd.cyou

[Q88] 行转列（条件聚合）
来源：http://tot.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cmd.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qzc.xziqi.cn

[Q89] 判断表是否存在
来源：http://yfe.ydjk.org.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hyp.gaohongyu789.top

[Q90] 生成序号列
来源：http://eog.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mwg.sufxvd.cn

================================================================================
来源：http://yvt.jqgfzy.top

R. Bash 专题
来源：http://hii.nanxinkj.top

================================================================================
来源：http://nea.52xcode.cn

[R01] shebang 与严格模式
来源：http://irt.hfpthk.cn

#!/usr/bin/env bash
来源：http://liv.aizwys.cn

set -euo pipefail
来源：http://eep.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://jsf.hammf.cn

name="Tom"; echo "$name"
来源：http://aqm.yonumen.top

[R03] 只读变量
来源：http://vdy.chenzaomai.com

readonly PI=3.14
来源：http://ufv.sjlbkw.cn

[R04] 位置参数
来源：http://psz.sufxvd.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://coz.jinqigfzy.top

[R05] 参数默认值
来源：http://xdn.zhengqikj.top

name="${1:-default}"
来源：http://sbn.yj202588.top

[R06] 判断命令是否存在
来源：http://rir.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jsx.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://sbl.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vks.yuxming.cn

[R08] 数值比较
来源：http://vmv.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://enh.ydzc1.top

[R09] 字符串比较
来源：http://llz.0kj1m.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jye.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://ptl.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vwi.redwolf501.top

[R11] case 多分支
来源：http://nlo.epnwcf.com

case "$1" in
来源：http://hcd.chenzaomai.com

start) echo "启动" ;;
来源：http://hae.shangyingyoupin.top

stop)  echo "停止" ;;
来源：http://yec.yonumen.top

*)     echo "未知命令" ;;
来源：http://jew.hysaishi.cn

esac
来源：http://chf.jinqigufen.top

[R12] for 遍历文件
来源：http://ian.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://onw.yj202588.top

[R13] for 计数循环
来源：http://rte.cdnleiting.top

for i in {1..10}; do echo "$i"; done
来源：http://wxa.zhixingplan.top

[R14] C 风格 for
来源：http://owx.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zta.epnwcf.com

[R15] while 逐行读文件
来源：http://pmz.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://exi.quarkkingdee.top

[R16] until 等待条件
来源：http://dbb.nanxinkj.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wya.smart0.xyz

[R17] 数组定义与取值
来源：http://tkk.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://pbc.yj20258.top

[R18] 遍历数组
来源：http://tkr.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hef.yj202588.top

[R19] 数组长度
来源：http://ygx.mhx1999.top

echo "${#arr[@]}"
来源：http://czz.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://lzb.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vbx.yj20258888.top

[R21] 字符串长度
来源：http://dto.zhixingplan.top

echo "${#s}"
来源：http://cfp.andypj.xyz

[R22] 截取子串
来源：http://nqn.smart0.xyz

echo "${s:0:5}"
来源：http://cvg.jqgfzy.top

[R23] 字符串替换
来源：http://vpk.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://enf.quarkkingdee.top

[R24] 大小写转换
来源：http://arv.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://osp.guowangkeji.top

[R25] 去后缀 / 去前缀
来源：http://kto.fengsongda.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cfo.epnwcf.com

[R26] 命令替换
来源：http://ktt.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://uqc.hywenlv.cn

[R27] 算术展开
来源：http://wyn.316326.xyz

echo $((1 + 2 * 3))
来源：http://aex.zhongyouzk.top

[R28] 浮点运算
来源：http://rxt.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://jle.yj202588.top

[R29] 定义函数
来源：http://zvb.yueranfly.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oqy.gzhubu.top

[R30] 函数返回状态码
来源：http://zru.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://rpx.xuanzx.com

[R31] 局部变量
来源：http://gxh.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://fpz.tian-w.cn

[R32] 参数个数校验
来源：http://kke.shuidangran.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wlz.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://yah.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://exp.andypj.xyz

[R34] 退出时清理
来源：http://tcy.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mes.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://qdx.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://psr.hesvh.cn

[R36] 并发执行多个任务
来源：http://bvq.bbcook.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mln.yonumen.top

[R37] 把输出赋给变量
来源：http://mzo.andypj.xyz

files=$(ls -1)
来源：http://ehx.andypj.xyz

[R38] 管道串联
来源：http://lbw.jyoumei.cn

cat a.txt | grep -i error | wc -l
来源：http://oja.yueranfly.top

[R39] 重定向标准输出与错误
来源：http://mzd.xuanzx.com

cmd > out.log 2>&1
来源：http://dab.jianghu66.top

[R40] 追加写日志
来源：http://psy.xylfe.cn

echo "log" >> out.log
来源：http://rmk.cheryme.top

[R41] 丢弃输出
来源：http://ysl.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://xlu.zdqjudy.top

[R42] 输入重定向
来源：http://hza.gaohongyu789.top

wc -l < a.txt
来源：http://iyz.hnxiangtu.top

[R43] 按名字查找文件
来源：http://lvv.shuidangran.top

find . -name "*.log" -type f
来源：http://agj.zdbjq.cn

[R44] 按修改时间查找
来源：http://oxe.jqgufenzy.top

find . -mtime -7 -type f
来源：http://luq.snrcjt.cn

[R45] 批量删除
来源：http://jnt.cashguo.top

find . -name "*.tmp" -delete
来源：http://ztr.havefunace.top

[R46] 递归替换文件内容
来源：http://imq.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uzn.kuanghao11.cn

[R47] sed 单行替换
来源：http://tnx.ydjk.org.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uzf.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://gmc.uphjek.com

awk '{print $1, $3}' a.txt
来源：http://pdv.vqdsnc.cn

[R49] awk 带条件
来源：http://czg.yuanzhike.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hco.cashguo.top

[R50] awk 求和
来源：http://igc.hesvh.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gdc.hesvh.cn

[R51] 排序去重取前几
来源：http://xuk.fengsongda.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vgk.0kj1m.cn

[R52] 统计行数
来源：http://jzo.yj202588.top

wc -l a.txt
来源：http://xfi.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://aqo.xziqi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zit.mhx1999.top

[R54] 比较两个文件
来源：http://vbu.havefunace.top

diff a.txt b.txt
来源：http://ilz.nanxinkj.top

[R55] 压缩与解压
来源：http://pzg.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://amb.bbcook.cn

[R56] 远程拷贝
来源：http://aca.vqdsnc.cn

scp file user@host:/path/
来源：http://key.jinqigufen.top

[R57] 远程执行命令
来源：http://wrj.yj20258888.top


<!-- 参考信息 -->