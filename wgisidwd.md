代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://xsf.52xcode.cn

[Q05] 重命名列
来源：http://jos.yuanzhike.top

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://xbq.dianchejie.cn

[Q06] 删除列
来源：http://rtb.9152youxi.cn

ALTER TABLE users DROP COLUMN age;
来源：http://nrq.pengpengdd.cyou

[Q07] 删除表
来源：http://yrl.meibo888.top

DROP TABLE IF EXISTS orders;
来源：http://kkl.hfpthk.cn

[Q08] 创建普通索引
来源：http://wmo.wangshuangyany.cn

CREATE INDEX idx_users_email ON users(email);
来源：http://ygs.jinqigfzy.top

[Q09] 创建唯一索引
来源：http://gxn.xingfuxueyuan.xyz

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://evs.meibo888.top

[Q10] 插入单行
来源：http://nkh.hcnkem.com

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wbc.aibaodan.cn

[Q11] 一次插入多行
来源：http://chl.tarul.cn

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://yiq.shanyushiyangkeji.top

[Q12] 插入后取自增 ID
来源：http://xma.jinqigfzy.top

INSERT INTO users (name) VALUES ('C');
来源：http://oug.xziqi.cn

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://pco.jlsjyb.cn

[Q13] 忽略重复插入
来源：http://bmq.cashguo.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://lxt.shangyingyoupin.top

[Q14] 存在则更新（upsert）
来源：http://iid.gzhubu.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wrg.cashguo.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://bil.xuanzx.com

[Q15] 查询全部
来源：http://pib.fehbvm.com

SELECT * FROM users;
来源：http://uzf.yj20258.top

[Q16] 查询指定列
来源：http://srw.hongshengwenyu.top

SELECT id, name FROM users;
来源：http://gcm.tanke756.top

[Q17] 条件查询
来源：http://tka.chenzaomai.com

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://hnm.bbcook.cn

[Q18] 模糊匹配
来源：http://pes.jinyuanbaomall.cn

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qqf.jqgufenzy.top

[Q19] 范围查询
来源：http://gmv.wangdashe.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://kuo.yonumen.top

[Q20] IN 列表
来源：http://xjp.yfazqb.com

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://cki.ydjk.org.cn

[Q21] 空值判断
来源：http://ing.jlsjyb.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://gwh.cashguo.top

[Q22] 排序
来源：http://gvj.jinghuilouyu.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wae.gaohongyu789.top

[Q23] 分页
来源：http://cfq.nanxinkj.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xfd.yanxiufei.cn

[Q24] 去重
来源：http://uni.xingfuxueyuan.xyz

SELECT DISTINCT city FROM users;
来源：http://wrh.chenzaomai.com

[Q25] 只取前 N 条
来源：http://gra.mhx1999.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://irf.yuanzhike.top

[Q26] 计数
来源：http://auv.mhx1999.top

SELECT COUNT(*) FROM users;
来源：http://phh.shuidangran.top

[Q27] 条件计数
来源：http://xub.yj20258.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://arn.ydzc1.top

[Q28] 求和与平均
来源：http://sxp.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://ppd.sweek.top

[Q29] 最大最小值
来源：http://xlk.cqqwz.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dpu.jinghuilouyu.cn

[Q30] 分组统计
来源：http://vbs.zdqjudy.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://aly.kuanghao11.cn

[Q31] 分组后过滤
来源：http://gap.quarkkingdee.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://psz.chenzaomai.com

[Q32] 分组拼接字符串
来源：http://rqg.ehwqpu.com

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://lsx.hfpthk.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://and.havefunace.top

[Q33] 多列分组
来源：http://xaq.hongshengwenyu.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ctd.yangfankeji.com

[Q34] 每组取第一条
来源：http://aum.cdnleiting.top

SELECT * FROM (
来源：http://tfc.jinqigufen.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://miu.gaohongyu789.top

) t WHERE rn = 1;
来源：http://nbu.guowangkeji.top

[Q35] 内连接
来源：http://cqk.ywan-chungtsiang.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://kai.fanxiaobao.xyz

[Q36] 左连接
来源：http://cqp.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://epb.tianlin.xyz

[Q37] 右连接
来源：http://naf.xziqi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://dqp.zhoulong.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://iqn.shanyushiyangtech.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pmj.zhoulong.xyz

[Q39] 自连接（查上下级）
来源：http://vkz.jlsjyb.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://zcz.zhiwuduotai.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vbi.yuxming.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://zcz.9152youxi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qoa.0kj1m.cn

[Q41] 多表连接
来源：http://gzs.zhoulong.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://rjl.sysykeji.top

JOIN users u ON u.id = o.user_id
来源：http://voy.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://efb.yonumen.top

[Q42] 连接条件附加过滤
来源：http://wks.yangfankeji.com

SELECT u.name, o.amount FROM users u
来源：http://iui.cheryme.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ydr.hnxiangtu.top

[Q43] 标量子查询
来源：http://ixe.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jru.hcnkem.com

[Q44] IN 子查询
来源：http://irl.cqqwz.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mpi.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://plz.gaohongyu789.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://svk.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://jpm.xinyue.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rkr.shanyushiyangtech.top

[Q47] 与平均值比较
来源：http://mwf.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uve.pycfn.com

[Q48] CTE 公用表表达式
来源：http://mra.vqdsnc.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vpy.iojbl.cn

SELECT * FROM t WHERE c > 5;
来源：http://qit.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://ceg.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rdf.vqdsnc.cn

[Q50] 批量更新
来源：http://tax.ywan-chungtsiang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qkt.yj20258888.top

[Q51] 用子查询更新
来源：http://pkv.jinghuilouyu.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://maw.ydjk.org.cn

[Q52] 删除指定行
来源：http://ykz.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://fvz.sufxvd.cn

[Q53] 按条件删除
来源：http://xjp.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gsp.hammf.cn

[Q54] 清空表
来源：http://xjd.nanxuanxn.top

TRUNCATE TABLE logs;
来源：http://awp.yanxiufei.cn

[Q55] 排名（并列占位）
来源：http://tjh.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nds.chenlongwang.top

[Q56] 密集排名（并列不占位）
来源：http://bkh.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nch.tarul.cn

[Q57] 行号
来源：http://nzh.shangyingyoupin.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://fly.dianchejie.cn

[Q58] 累计求和
来源：http://vfr.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://zov.daria6918.cn

[Q59] 分组内累计
来源：http://jrn.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yhr.hongshengwenyu.top

[Q60] 取上一行 / 下一行
来源：http://tlt.zhengqikj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zdy.nanxuanxn.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qeu.jinqigufen.top

[Q61] 移动平均
来源：http://pji.wangdashe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wyo.haohaochexian.top

[Q62] 分组占比
来源：http://toa.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xsi.jinghuilouyu.cn

[Q63] 开启事务
来源：http://wuy.zhijiandao.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jox.iojbl.cn

[Q64] 提交事务
来源：http://luk.kuanghao11.cn

COMMIT;
来源：http://rme.ywan-chungtsiang.top

[Q65] 回滚事务
来源：http://lcd.ywan-chungtsiang.top

ROLLBACK;
来源：http://atl.cdnleiting.top

[Q66] 行锁查询
来源：http://klg.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nri.fehbvm.com

[Q67] 设置隔离级别
来源：http://xvz.zhaomingkeji.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jht.yuanzhike.top

[Q68] 保存点
来源：http://wwf.iojbl.cn

SAVEPOINT sp1;
来源：http://bnw.sxryk.cn

ROLLBACK TO sp1;
来源：http://zfh.svipenyu.cn

[Q69] 查看执行计划
来源：http://qoi.chenlongwang.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://iic.vehdjk.com

[Q70] 更新统计信息
来源：http://tav.chenzaomai.com

ANALYZE TABLE users;
来源：http://kpr.yonumen.top

[Q71] 查看建表语句
来源：http://azg.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ptq.chenlongwang.top

[Q72] 查看索引
来源：http://yfp.xinyue.icu

SHOW INDEX FROM users;
来源：http://wdc.hfpthk.cn

[Q73] 查看表状态
来源：http://gsv.xuanzx.com

SHOW TABLE STATUS LIKE 'users';
来源：http://bdr.cheryme.top

[Q74] 强制使用索引
来源：http://cwl.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vaa.svipenyu.cn

[Q75] 日期格式化
来源：http://xar.xinyue.icu

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uvp.gaohongyu789.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jmo.zhiwuduotai.top

[Q76] 按天统计
来源：http://drh.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yfb.svipenyu.cn

[Q77] 时间加减
来源：http://fnu.hfpthk.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ecq.0kj1m.cn

[Q78] 当前时间
来源：http://xvn.hysaishi.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aia.hysaishi.cn

[Q79] 字符串拼接
来源：http://woc.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pct.c1oappe.top

[Q80] 字符串截取
来源：http://gpg.gogol.net.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mdf.yangfankeji.com

[Q81] 字符串替换
来源：http://kgl.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://sbs.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://nbl.chenlongwang.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rbn.iojbl.cn

[Q83] 大小写转换
来源：http://tei.yfazqb.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tns.9152youxi.cn

[Q84] 去除首尾空格
来源：http://owe.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://edt.yuanzhike.top

[Q85] 数值取整
来源：http://hkj.zhengqikj.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://noz.tarul.cn

[Q86] 读取 JSON 字段
来源：http://wub.svipenyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jkd.daxiang520.top

[Q87] JSON 字段做条件
来源：http://ywr.bjfxy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iez.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://dcy.yuxming.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pzz.chenzaomai.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bhn.jqgfzy.top

[Q89] 判断表是否存在
来源：http://btx.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rht.fanxiaobao.xyz

[Q90] 生成序号列
来源：http://img.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ufv.zhijiandao.cn

================================================================================
来源：http://ulx.wangdashe.top

R. Bash 专题
来源：http://xgu.ivvv.top

================================================================================
来源：http://bbv.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://zvg.yuanzhike.top

#!/usr/bin/env bash
来源：http://zfr.zhaomingkeji.xyz

set -euo pipefail
来源：http://rmu.shanyushiyangkeji.top

[R02] 变量赋值与使用
来源：http://agi.ybcxt.top

name="Tom"; echo "$name"
来源：http://ulm.vehdjk.com

[R03] 只读变量
来源：http://mck.havefunace.top

readonly PI=3.14
来源：http://xbn.ywan-chungtsiang.top

[R04] 位置参数
来源：http://xkq.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://msd.fengsongda.top

[R05] 参数默认值
来源：http://ioo.yuanzhike.top

name="${1:-default}"
来源：http://oov.52xcode.cn

[R06] 判断命令是否存在
来源：http://hjl.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mgh.fehbvm.com

[R07] if 判断文件
来源：http://mpf.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lbc.wangdashe.top

[R08] 数值比较
来源：http://srk.yfazqb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://oqw.hammf.cn

[R09] 字符串比较
来源：http://qhe.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yfx.fanxiaobao.xyz

[R10] 正则匹配
来源：http://onw.xylfe.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dkk.yongpay.top

[R11] case 多分支
来源：http://ywo.hnqzz.top

case "$1" in
来源：http://pbe.redwolf501.top

start) echo "启动" ;;
来源：http://jii.havefunace.top

stop)  echo "停止" ;;
来源：http://yei.jqgufenzy.top

*)     echo "未知命令" ;;
来源：http://uya.jiagoushi.top

esac
来源：http://rrw.smart0.xyz

[R12] for 遍历文件
来源：http://ffn.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://sdj.sjlbkw.cn

[R13] for 计数循环
来源：http://ulh.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://cfh.bjfxy.top

[R14] C 风格 for
来源：http://zdm.tarul.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://stv.hnqzz.top

[R15] while 逐行读文件
来源：http://qmv.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://htk.sysykeji.top

[R16] until 等待条件
来源：http://cgo.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uaq.tianlin.xyz

[R17] 数组定义与取值
来源：http://bcq.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ddt.sweek.top

[R18] 遍历数组
来源：http://yvv.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vwb.mhx1999.top

[R19] 数组长度
来源：http://mcb.yonumen.top

echo "${#arr[@]}"
来源：http://uoy.jyoumei.cn

[R20] 关联数组（字典）
来源：http://ovh.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dqp.yueranfly.top

[R21] 字符串长度
来源：http://egt.bjfxy.top

echo "${#s}"
来源：http://zkq.hysaishi.cn

[R22] 截取子串
来源：http://zyg.jianghu66.top

echo "${s:0:5}"
来源：http://xbw.ppjwa.cn

[R23] 字符串替换
来源：http://ysj.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fhd.xinyue.icu

[R24] 大小写转换
来源：http://mhh.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://tog.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://goa.zhengqikj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pob.gotoacloud.top

[R26] 命令替换
来源：http://ygp.tanke756.top

now=$(date +%F); echo "$now"
来源：http://zda.cucudq.cn

[R27] 算术展开
来源：http://uqw.yfazqb.com

echo $((1 + 2 * 3))
来源：http://qzy.jinqigufen.top

[R28] 浮点运算
来源：http://tld.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://ggn.yueranfly.top

[R29] 定义函数
来源：http://tsi.zhiwuduotai.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mis.quarkkingdee.top

[R30] 函数返回状态码
来源：http://dnm.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://iop.0kj1m.cn

[R31] 局部变量
来源：http://uun.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://gdj.sufxvd.cn

[R32] 参数个数校验
来源：http://zce.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iss.quarkkingdee.top

[R33] 捕获错误并提示行号
来源：http://zxm.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://arv.jianghu66.top

[R34] 退出时清理
来源：http://lhz.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://osp.kuanghao11.cn

[R35] 后台执行并等待
来源：http://ccv.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://clu.aizwys.cn

[R36] 并发执行多个任务
来源：http://xik.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jdi.svipenyu.cn

[R37] 把输出赋给变量
来源：http://oml.hysaishi.cn

files=$(ls -1)
来源：http://nrh.yuxming.cn

[R38] 管道串联
来源：http://mef.cashguo.top

cat a.txt | grep -i error | wc -l
来源：http://eql.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://prx.cheryme.top

cmd > out.log 2>&1
来源：http://fdv.yueranfly.top

[R40] 追加写日志
来源：http://bmp.tianlin.xyz

echo "log" >> out.log
来源：http://whu.ybcxt.top

[R41] 丢弃输出
来源：http://ans.haohaochexian.top

cmd >/dev/null 2>&1
来源：http://ixf.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://bwf.hongshengwenyu.top

wc -l < a.txt
来源：http://sfy.316326.xyz

[R43] 按名字查找文件
来源：http://jod.yuanzhike.top

find . -name "*.log" -type f
来源：http://tqv.jinqigufen.top

[R44] 按修改时间查找
来源：http://rbh.jinqigfzy.top

find . -mtime -7 -type f
来源：http://moa.jiagoushi.top

[R45] 批量删除
来源：http://qdl.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://abo.jiagoushi.top

[R46] 递归替换文件内容
来源：http://zmu.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tyv.iojbl.cn

[R47] sed 单行替换
来源：http://biw.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://dcz.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://cxy.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://hby.sweek.top

[R49] awk 带条件
来源：http://mik.cashguo.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iem.andypj.xyz

[R50] awk 求和
来源：http://qbo.xylfe.cn

awk '{s += $2} END {print s}' a.txt
来源：http://znt.yuxming.cn

[R51] 排序去重取前几
来源：http://xzw.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rwv.jiagoushi.top

[R52] 统计行数
来源：http://psl.smart0.xyz

wc -l a.txt
来源：http://uhk.yvedp.cn

[R53] 查看文件头与实时尾
来源：http://lpd.pengpengdd.cyou


<!-- 参考信息 -->