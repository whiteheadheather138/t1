代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://tjp.fehbvm.com

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://ucx.ybcxt.top

[Q13] 忽略重复插入
来源：http://wav.yueranfly.top

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://iqp.yanxiufei.cn

[Q14] 存在则更新（upsert）
来源：http://fvn.cashguo.top

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://hvk.xuanzx.com

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://isg.snrcjt.cn

[Q15] 查询全部
来源：http://qsa.tarul.cn

SELECT * FROM users;
来源：http://ccx.yangfankeji.com

[Q16] 查询指定列
来源：http://pqd.ydzc1.top

SELECT id, name FROM users;
来源：http://ezy.cdnleiting.top

[Q17] 条件查询
来源：http://cqd.cheryme.top

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wgf.aibaodan.cn

[Q18] 模糊匹配
来源：http://whf.smart0.xyz

SELECT * FROM users WHERE name LIKE '张%';
来源：http://qtr.gogol.net.cn

[Q19] 范围查询
来源：http://hhq.jianghu66.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://gji.zhengqikj.top

[Q20] IN 列表
来源：http://tjy.bjfxy.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://dwi.guowangkeji.top

[Q21] 空值判断
来源：http://enm.jiagoushi.top

SELECT * FROM users WHERE email IS NULL;
来源：http://szh.meibo888.top

[Q22] 排序
来源：http://gsu.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://rvd.ehwqpu.com

[Q23] 分页
来源：http://hqh.ywan-chungtsiang.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wjg.andypj.xyz

[Q24] 去重
来源：http://zsq.zhoulong.xyz

SELECT DISTINCT city FROM users;
来源：http://ggl.shanyushiyangtech.top

[Q25] 只取前 N 条
来源：http://koa.yueranfly.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://qfl.xinyue.icu

[Q26] 计数
来源：http://bmg.chenzaomai.com

SELECT COUNT(*) FROM users;
来源：http://cha.svipenyu.cn

[Q27] 条件计数
来源：http://gnd.gaohongyu789.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rby.yuanzhike.top

[Q28] 求和与平均
来源：http://qit.hywenlv.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://zce.ppjwa.cn

[Q29] 最大最小值
来源：http://jkl.xuanzx.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://umd.zdbjq.cn

[Q30] 分组统计
来源：http://kmp.wangdashe.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://xoq.0kj1m.cn

[Q31] 分组后过滤
来源：http://wke.c1oappe.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://ysa.hfpthk.cn

[Q32] 分组拼接字符串
来源：http://qsh.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://twn.wangshuangyany.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://oii.birdmap.top

[Q33] 多列分组
来源：http://aor.gogol.net.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://hqw.shzxlz.cn

[Q34] 每组取第一条
来源：http://xda.yanxiufei.cn

SELECT * FROM (
来源：http://mtb.zhengqikj.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://fyv.dianchejie.cn

) t WHERE rn = 1;
来源：http://xdw.cqqwz.cn

[Q35] 内连接
来源：http://vlg.xinyue.icu

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://bvp.xinyue.icu

[Q36] 左连接
来源：http://otx.vqdsnc.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://okt.yvedp.cn

[Q37] 右连接
来源：http://bfk.nanxinkj.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://qci.wangshuangyany.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kti.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qzx.hnqzz.top

[Q39] 自连接（查上下级）
来源：http://wdf.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cqr.zhijiandao.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://rpe.shangyingyoupin.top

[Q40] 交叉连接（笛卡尔积）
来源：http://hoc.wangshuangyany.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://veb.hywenlv.cn

[Q41] 多表连接
来源：http://fkv.yvedp.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://qzz.dianchejie.cn

JOIN users u ON u.id = o.user_id
来源：http://rgz.gotoacloud.top

JOIN products p ON p.id = o.product_id;
来源：http://csu.cdnleiting.top

[Q42] 连接条件附加过滤
来源：http://nxt.hongshengwenyu.top

SELECT u.name, o.amount FROM users u
来源：http://jyx.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uyq.zhiwuduotai.top

[Q43] 标量子查询
来源：http://cki.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://uqs.jinghuilouyu.cn

[Q44] IN 子查询
来源：http://lxa.xuetiantiany.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ftb.xinyue.icu

[Q45] EXISTS 判断存在
来源：http://vzl.jinqigufen.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ifn.tianlin.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://lww.aizwys.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://omn.fehbvm.com

[Q47] 与平均值比较
来源：http://whi.jinghuilouyu.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pfm.jinghuilouyu.cn

[Q48] CTE 公用表表达式
来源：http://anv.yanxiufei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://bmh.xziqi.cn

SELECT * FROM t WHERE c > 5;
来源：http://mhr.yj20258888.top

[Q49] 更新单行
来源：http://tlm.zdqjudy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ngs.c1oappe.top

[Q50] 批量更新
来源：http://wjv.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://bsw.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://wtq.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwj.shanyushiyangkeji.top

[Q52] 删除指定行
来源：http://qxa.tanke756.top

DELETE FROM users WHERE id = 10;
来源：http://gfv.iojbl.cn

[Q53] 按条件删除
来源：http://zyl.guowangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bbw.kuanghao11.cn

[Q54] 清空表
来源：http://sns.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://prd.cucudq.cn

[Q55] 排名（并列占位）
来源：http://qfw.sysykeji.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hsl.fanxiaobao.xyz

[Q56] 密集排名（并列不占位）
来源：http://nip.yanxiufei.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eky.chenjidiqi.icu

[Q57] 行号
来源：http://dzu.zhongyouzk.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uwy.dashuyun.cn

[Q58] 累计求和
来源：http://pae.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bnt.epnwcf.com

[Q59] 分组内累计
来源：http://ghu.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mua.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://vpk.hcnkem.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://veu.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jli.wangdashe.top

[Q61] 移动平均
来源：http://vry.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://koq.smart0.xyz

[Q62] 分组占比
来源：http://ivm.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://byy.jinghuilouyu.cn

[Q63] 开启事务
来源：http://nxv.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://avh.xylfe.cn

[Q64] 提交事务
来源：http://adw.yongpay.top

COMMIT;
来源：http://gdy.jqgfzy.top

[Q65] 回滚事务
来源：http://qdq.shanyushiyangkeji.top

ROLLBACK;
来源：http://mlo.iojbl.cn

[Q66] 行锁查询
来源：http://mtp.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hjz.fzhhl.top

[Q67] 设置隔离级别
来源：http://vxw.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hul.yueranfly.top

[Q68] 保存点
来源：http://mhn.quarkkingdee.top

SAVEPOINT sp1;
来源：http://gbn.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://shw.cdnleiting.top

[Q69] 查看执行计划
来源：http://ibr.nanxuanxn.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ypo.sysykeji.top

[Q70] 更新统计信息
来源：http://mea.yj20258.top

ANALYZE TABLE users;
来源：http://wnb.fengsongda.top

[Q71] 查看建表语句
来源：http://zml.cdnleiting.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xxn.gaohongyu789.top

[Q72] 查看索引
来源：http://mvs.jyoumei.cn

SHOW INDEX FROM users;
来源：http://syy.fktsv.cn

[Q73] 查看表状态
来源：http://lol.bbcook.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rmj.wangdashe.top

[Q74] 强制使用索引
来源：http://kmj.cucudq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lyp.yj20258.top

[Q75] 日期格式化
来源：http://cbh.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ctg.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ezt.zhengqikj.top

[Q76] 按天统计
来源：http://xmx.zhongyouzk.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vbp.iojbl.cn

[Q77] 时间加减
来源：http://ram.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zbx.pycfn.com

[Q78] 当前时间
来源：http://olz.gotoacloud.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://igs.gotoacloud.top

[Q79] 字符串拼接
来源：http://bpe.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://omd.bbcook.cn

[Q80] 字符串截取
来源：http://hep.dianchejie.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wkz.fengsongda.top

[Q81] 字符串替换
来源：http://rek.yonumen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://grb.yvedp.cn

[Q82] 字符长度与字节长度
来源：http://ejt.tarul.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://nro.svipenyu.cn

[Q83] 大小写转换
来源：http://lhx.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bse.wangdashe.top

[Q84] 去除首尾空格
来源：http://oqc.fanxiaobao.xyz

SELECT TRIM(name) FROM users;
来源：http://ssy.cashguo.top

[Q85] 数值取整
来源：http://tpk.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://siv.0kj1m.cn

[Q86] 读取 JSON 字段
来源：http://api.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ysj.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://xgr.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fvf.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://pho.feifeiyinyue.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gql.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wzw.xingfuxueyuan.xyz

[Q89] 判断表是否存在
来源：http://mqm.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rog.shzxlz.cn

[Q90] 生成序号列
来源：http://uad.meibo888.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pso.guowangkeji.top

================================================================================
来源：http://rud.jianghu66.top

R. Bash 专题
来源：http://rnr.shanyushiyangkeji.top

================================================================================
来源：http://jbb.xuetiantiany.cn

[R01] shebang 与严格模式
来源：http://bdc.gzhubu.top

#!/usr/bin/env bash
来源：http://lyi.shuidangran.top

set -euo pipefail
来源：http://mhy.xuanzx.com

[R02] 变量赋值与使用
来源：http://wpd.yueranfly.top

name="Tom"; echo "$name"
来源：http://xqp.yueranfly.top

[R03] 只读变量
来源：http://ino.sweek.top

readonly PI=3.14
来源：http://kep.wangdashe.top

[R04] 位置参数
来源：http://nxx.vqdsnc.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ogv.jqgufenzy.top

[R05] 参数默认值
来源：http://eiq.yanxiufei.cn

name="${1:-default}"
来源：http://tdu.hfpthk.cn

[R06] 判断命令是否存在
来源：http://igc.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rtk.cdnleiting.top

[R07] if 判断文件
来源：http://tii.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ytk.yfazqb.com

[R08] 数值比较
来源：http://mph.haohaochexian.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ihb.c1oappe.top

[R09] 字符串比较
来源：http://hev.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cxb.jinqigufen.top

[R10] 正则匹配
来源：http://pkg.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uuz.zhijiandao.cn

[R11] case 多分支
来源：http://rgj.jianghu66.top

case "$1" in
来源：http://ght.uphjek.com

start) echo "启动" ;;
来源：http://zum.jiagoushi.top

stop)  echo "停止" ;;
来源：http://tza.yanxiufei.cn

*)     echo "未知命令" ;;
来源：http://abw.chenlongwang.top

esac
来源：http://cji.xziqi.cn

[R12] for 遍历文件
来源：http://grp.yj202588.top

for f in *.txt; do echo "$f"; done
来源：http://yud.cheryme.top

[R13] for 计数循环
来源：http://ppf.jqgfzy.top

for i in {1..10}; do echo "$i"; done
来源：http://mpu.c1oappe.top

[R14] C 风格 for
来源：http://buv.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xbt.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://dab.ywan-chungtsiang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://urc.zdbjq.cn

[R16] until 等待条件
来源：http://ius.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rrm.mhx1999.top

[R17] 数组定义与取值
来源：http://ggm.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dlc.gogol.net.cn

[R18] 遍历数组
来源：http://pcs.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kep.cqqwz.cn

[R19] 数组长度
来源：http://jhw.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://moi.kuanghao11.cn

[R20] 关联数组（字典）
来源：http://kkm.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ebq.snrcjt.cn

[R21] 字符串长度
来源：http://rra.jlsjyb.cn

echo "${#s}"
来源：http://vdz.xziqi.cn

[R22] 截取子串
来源：http://ytt.xziqi.cn

echo "${s:0:5}"
来源：http://rey.hesvh.cn

[R23] 字符串替换
来源：http://ehr.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qbi.bbcook.cn

[R24] 大小写转换
来源：http://bix.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://tag.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://zxh.ydjk.org.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pev.c1oappe.top

[R26] 命令替换
来源：http://lzu.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://cfl.sjlbkw.cn

[R27] 算术展开
来源：http://ovh.316326.xyz

echo $((1 + 2 * 3))
来源：http://pqz.yanxiufei.cn

[R28] 浮点运算
来源：http://jez.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://ucx.jinyuanbaomall.cn

[R29] 定义函数
来源：http://xpc.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zel.jiagoushi.top

[R30] 函数返回状态码
来源：http://jsv.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://xgq.zycfv.cn

[R31] 局部变量
来源：http://lan.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://kae.fehbvm.com

[R32] 参数个数校验
来源：http://wss.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bno.vehdjk.com

[R33] 捕获错误并提示行号
来源：http://jtt.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sao.haohaochexian.top

[R34] 退出时清理
来源：http://pos.iojbl.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tcu.ydjk.org.cn

[R35] 后台执行并等待
来源：http://gdp.shuidangran.top

sleep 5 & pid=$!; wait "$pid"
来源：http://edx.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://lko.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bra.hysaishi.cn

[R37] 把输出赋给变量
来源：http://feg.quarkkingdee.top

files=$(ls -1)
来源：http://sls.yanxiufei.cn

[R38] 管道串联
来源：http://ale.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://iik.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://vko.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://uzg.aibaodan.cn

[R40] 追加写日志
来源：http://wqg.daria6918.cn

echo "log" >> out.log
来源：http://ahu.hysaishi.cn

[R41] 丢弃输出
来源：http://esc.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://kkb.zycfv.cn

[R42] 输入重定向
来源：http://dqe.ehwqpu.com

wc -l < a.txt
来源：http://iqf.hnqzz.top

[R43] 按名字查找文件
来源：http://unj.gotoacloud.top

find . -name "*.log" -type f
来源：http://edc.zhongyouzk.top

[R44] 按修改时间查找
来源：http://vow.jinqigfzy.top

find . -mtime -7 -type f
来源：http://lwx.yongpay.top

[R45] 批量删除
来源：http://zsg.meibo888.top

find . -name "*.tmp" -delete
来源：http://xxx.jyoumei.cn

[R46] 递归替换文件内容
来源：http://piq.gaohongyu789.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ogn.hesvh.cn

[R47] sed 单行替换
来源：http://gqz.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ksl.316326.xyz

[R48] awk 取指定列
来源：http://npe.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://kqd.fengsongda.top

[R49] awk 带条件
来源：http://bhu.fanxiaobao.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iav.sufxvd.cn

[R50] awk 求和
来源：http://lcl.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://zny.yuxming.cn

[R51] 排序去重取前几
来源：http://ysc.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ils.zhengqikj.top

[R52] 统计行数
来源：http://hju.jianghu66.top

wc -l a.txt
来源：http://efq.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://zmb.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wbs.hcnkem.com

[R54] 比较两个文件
来源：http://zsu.fehbvm.com

diff a.txt b.txt
来源：http://usn.zhoulong.xyz

[R55] 压缩与解压
来源：http://rze.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dxi.nwbrower.top

[R56] 远程拷贝
来源：http://wpv.yangfankeji.com

scp file user@host:/path/
来源：http://gpl.yuxming.cn

[R57] 远程执行命令
来源：http://hhf.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://sjc.redwolf501.top

[R58] 下载文件
来源：http://rtb.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iyu.cashguo.top

[R59] 发 POST JSON
来源：http://ifd.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ezq.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://hri.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://skr.ydzc1.top

[R61] 磁盘占用
来源：http://bhv.bjfxy.top


<!-- 参考信息 -->