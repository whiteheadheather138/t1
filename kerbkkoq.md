代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://zkf.sysykeji.top

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://uvt.sufxvd.cn

[Q13] 忽略重复插入
来源：http://zfp.zhaomingkeji.xyz

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://rdq.quarkkingdee.top

[Q14] 存在则更新（upsert）
来源：http://urt.svipenyu.cn

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://uje.zhixingplan.top

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://jdx.jqgfzy.top

[Q15] 查询全部
来源：http://jrs.jinghuilouyu.cn

SELECT * FROM users;
来源：http://feu.sysykeji.top

[Q16] 查询指定列
来源：http://zdu.svipenyu.cn

SELECT id, name FROM users;
来源：http://tly.smart0.xyz

[Q17] 条件查询
来源：http://ssf.sufxvd.cn

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://coa.ctjpmb.com

[Q18] 模糊匹配
来源：http://zas.yuanzhike.top

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bfw.hnxiangtu.top

[Q19] 范围查询
来源：http://hsh.52xcode.cn

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://bba.hnxiangtu.top

[Q20] IN 列表
来源：http://cnl.fengsongda.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mdp.kuanghao11.cn

[Q21] 空值判断
来源：http://jqx.snrcjt.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://kjy.ppjwa.cn

[Q22] 排序
来源：http://scp.0kj1m.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://urw.hnqzz.top

[Q23] 分页
来源：http://zur.cashguo.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://xnu.wangdashe.top

[Q24] 去重
来源：http://vah.hywenlv.cn

SELECT DISTINCT city FROM users;
来源：http://qkf.zhiwuduotai.top

[Q25] 只取前 N 条
来源：http://keu.yj202588.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://uaa.xuetiantiany.cn

[Q26] 计数
来源：http://jhp.uphjek.com

SELECT COUNT(*) FROM users;
来源：http://ozc.ppjwa.cn

[Q27] 条件计数
来源：http://woh.zhixingplan.top

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vke.shanyushiyangkeji.top

[Q28] 求和与平均
来源：http://rhe.gzhubu.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://gpg.aizwys.cn

[Q29] 最大最小值
来源：http://sqy.tian-w.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://zyk.nanxuanxn.top

[Q30] 分组统计
来源：http://uxp.kuanghao11.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://hxr.nanxuanxn.top

[Q31] 分组后过滤
来源：http://sae.hywenlv.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://sdu.kuanghao11.cn

[Q32] 分组拼接字符串
来源：http://joj.gogol.net.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://bns.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://dql.316326.xyz

[Q33] 多列分组
来源：http://vcx.ppjwa.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://bzc.ydzc1.top

[Q34] 每组取第一条
来源：http://tuz.guannengcc.top

SELECT * FROM (
来源：http://jla.sysykeji.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://lla.shanyushiyangkeji.top

) t WHERE rn = 1;
来源：http://xsw.dashuyun.cn

[Q35] 内连接
来源：http://kcj.hongshengwenyu.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mcs.havefunace.top

[Q36] 左连接
来源：http://dnv.uphjek.com

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://izn.cucudq.cn

[Q37] 右连接
来源：http://fxr.zhixingplan.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://zpx.bbcook.cn

[Q38] 全外连接（PostgreSQL）
来源：http://mjf.ybcxt.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://oyz.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://owt.zhixingplan.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://rlj.jianghu66.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://oxq.yueranfly.top

[Q40] 交叉连接（笛卡尔积）
来源：http://mzl.hysaishi.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://zqk.wangshuangyany.cn

[Q41] 多表连接
来源：http://jcs.gotoacloud.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://zmw.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://ccd.sjlbkw.cn

JOIN products p ON p.id = o.product_id;
来源：http://cha.fzhhl.top

[Q42] 连接条件附加过滤
来源：http://log.bbcook.cn

SELECT u.name, o.amount FROM users u
来源：http://oyr.dashuyun.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://toh.0kj1m.cn

[Q43] 标量子查询
来源：http://rvg.tarul.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wqg.chenjidiqi.icu

[Q44] IN 子查询
来源：http://use.hywenlv.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://lmc.feifeiyinyue.top

[Q45] EXISTS 判断存在
来源：http://eyf.xinyue.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xym.shanyushiyangtech.top

[Q46] NOT EXISTS 判断不存在
来源：http://glo.quarkkingdee.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rvz.gzhubu.top

[Q47] 与平均值比较
来源：http://ohp.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ggy.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://ebg.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wrw.hammf.cn

SELECT * FROM t WHERE c > 5;
来源：http://jio.aibaodan.cn

[Q49] 更新单行
来源：http://hka.bjfxy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hra.ivvv.top

[Q50] 批量更新
来源：http://dmc.shzxlz.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cng.snrcjt.cn

[Q51] 用子查询更新
来源：http://glc.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oir.shanyushiyangtech.top

[Q52] 删除指定行
来源：http://jbc.ppjwa.cn

DELETE FROM users WHERE id = 10;
来源：http://gpf.316326.xyz

[Q53] 按条件删除
来源：http://urw.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://efn.yj20258.top

[Q54] 清空表
来源：http://zdf.hesvh.cn

TRUNCATE TABLE logs;
来源：http://kaz.yvedp.cn

[Q55] 排名（并列占位）
来源：http://nrv.hfpthk.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://rnh.yvedp.cn

[Q56] 密集排名（并列不占位）
来源：http://hbj.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://imd.chenzaomai.com

[Q57] 行号
来源：http://jhy.yangfankeji.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cqo.fanxiaobao.xyz

[Q58] 累计求和
来源：http://oaj.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fqv.gogol.net.cn

[Q59] 分组内累计
来源：http://gsb.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qvk.cheryme.top

[Q60] 取上一行 / 下一行
来源：http://qvy.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uhi.havefunace.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://kkl.zycfv.cn

[Q61] 移动平均
来源：http://irn.tianlin.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://syu.sxryk.cn

[Q62] 分组占比
来源：http://mzr.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lab.dashuyun.cn

[Q63] 开启事务
来源：http://kve.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fgx.tian-w.cn

[Q64] 提交事务
来源：http://twx.pengpengdd.cyou

COMMIT;
来源：http://rix.jianghu66.top

[Q65] 回滚事务
来源：http://nwj.gaohongyu789.top

ROLLBACK;
来源：http://exc.gotoacloud.top

[Q66] 行锁查询
来源：http://owb.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vbj.pengpengdd.cyou

[Q67] 设置隔离级别
来源：http://xno.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cvr.jqgufenzy.top

[Q68] 保存点
来源：http://uqh.yvedp.cn

SAVEPOINT sp1;
来源：http://qyq.yj20258888.top

ROLLBACK TO sp1;
来源：http://cym.9152youxi.cn

[Q69] 查看执行计划
来源：http://bwa.vehdjk.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fxa.dashuyun.cn

[Q70] 更新统计信息
来源：http://biv.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://rpf.yanxiufei.cn

[Q71] 查看建表语句
来源：http://gfe.andypj.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jvq.fzhhl.top

[Q72] 查看索引
来源：http://iqx.xziqi.cn

SHOW INDEX FROM users;
来源：http://wle.jinqigufen.top

[Q73] 查看表状态
来源：http://svn.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nmy.zhixingplan.top

[Q74] 强制使用索引
来源：http://ezn.gogol.net.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://srh.kuanghao11.cn

[Q75] 日期格式化
来源：http://zvn.bjfxy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://etq.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bzr.fzhhl.top

[Q76] 按天统计
来源：http://ucf.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dey.haohaochexian.top

[Q77] 时间加减
来源：http://kqx.zhijiandao.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sej.hongshengwenyu.top

[Q78] 当前时间
来源：http://wbb.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nmb.yj202588.top

[Q79] 字符串拼接
来源：http://ybd.hesvh.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://idl.fehbvm.com

[Q80] 字符串截取
来源：http://fzr.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://srn.jqgfzy.top

[Q81] 字符串替换
来源：http://zur.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://zwm.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://boh.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wxd.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://myg.smart0.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lca.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://nap.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://llk.shzxlz.cn

[Q85] 数值取整
来源：http://obv.epnwcf.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vdg.havefunace.top

[Q86] 读取 JSON 字段
来源：http://mgf.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tbu.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://hlw.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://yra.iojbl.cn

[Q88] 行转列（条件聚合）
来源：http://ptm.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xiu.gotoacloud.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zim.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://pfc.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ivd.hysaishi.cn

[Q90] 生成序号列
来源：http://bpl.zhiwuduotai.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cih.snrcjt.cn

================================================================================
来源：http://rhu.jlsjyb.cn

R. Bash 专题
来源：http://vcb.xylfe.cn

================================================================================
来源：http://vbt.sweek.top

[R01] shebang 与严格模式
来源：http://psx.xinyue.icu

#!/usr/bin/env bash
来源：http://ixz.jinghuilouyu.cn

set -euo pipefail
来源：http://rsg.shuidangran.top

[R02] 变量赋值与使用
来源：http://gvh.jqgufenzy.top

name="Tom"; echo "$name"
来源：http://nad.jyoumei.cn

[R03] 只读变量
来源：http://zhh.sysykeji.top

readonly PI=3.14
来源：http://yjk.jyoumei.cn

[R04] 位置参数
来源：http://pqx.daxiang520.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mpg.zhijiandao.cn

[R05] 参数默认值
来源：http://kox.jinqigfzy.top

name="${1:-default}"
来源：http://idl.snrcjt.cn

[R06] 判断命令是否存在
来源：http://hax.pengpengdd.cyou

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zbq.dianchejie.cn

[R07] if 判断文件
来源：http://hdx.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gro.zhoulong.xyz

[R08] 数值比较
来源：http://qin.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ksw.yj20258888.top

[R09] 字符串比较
来源：http://ncz.quarkkingdee.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qea.xingfuxueyuan.xyz

[R10] 正则匹配
来源：http://juz.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://czg.ybcxt.top

[R11] case 多分支
来源：http://yly.uphjek.com

case "$1" in
来源：http://ayj.jlsjyb.cn

start) echo "启动" ;;
来源：http://qwq.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://guc.yj20258888.top

*)     echo "未知命令" ;;
来源：http://tgk.guowangkeji.top

esac
来源：http://yxb.yj20258888.top

[R12] for 遍历文件
来源：http://fvy.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://rgr.yonumen.top

[R13] for 计数循环
来源：http://ttu.yuanzhike.top

for i in {1..10}; do echo "$i"; done
来源：http://ggu.smart0.xyz

[R14] C 风格 for
来源：http://jyf.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qcx.birdmap.top

[R15] while 逐行读文件
来源：http://vrg.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ifg.0kj1m.cn

[R16] until 等待条件
来源：http://uxd.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dwm.ybcxt.top

[R17] 数组定义与取值
来源：http://ccm.tarul.cn

arr=(a b c); echo "${arr[0]}"
来源：http://cat.cashguo.top

[R18] 遍历数组
来源：http://qgr.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fnf.sysykeji.top

[R19] 数组长度
来源：http://pgz.hysaishi.cn

echo "${#arr[@]}"
来源：http://mif.0kj1m.cn

[R20] 关联数组（字典）
来源：http://mhf.havefunace.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nbg.fktsv.cn

[R21] 字符串长度
来源：http://aip.yvedp.cn

echo "${#s}"
来源：http://fts.zhixingplan.top

[R22] 截取子串
来源：http://vft.tian-w.cn

echo "${s:0:5}"
来源：http://aom.yj20258.top

[R23] 字符串替换
来源：http://wxy.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kbx.kuanghao11.cn

[R24] 大小写转换
来源：http://zsa.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://zxn.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://rhk.hnxiangtu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hff.cucudq.cn

[R26] 命令替换
来源：http://qwi.xingfuxueyuan.xyz

now=$(date +%F); echo "$now"
来源：http://phx.bjfxy.top

[R27] 算术展开
来源：http://eqz.daria6918.cn

echo $((1 + 2 * 3))
来源：http://qvf.yueranfly.top

[R28] 浮点运算
来源：http://ehv.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://nbv.zhixingplan.top

[R29] 定义函数
来源：http://xrw.aibaodan.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lui.yonumen.top

[R30] 函数返回状态码
来源：http://yic.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://yby.cucudq.cn

[R31] 局部变量
来源：http://jrz.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://tqs.aizwys.cn

[R32] 参数个数校验
来源：http://ten.yj20258.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qau.feifeiyinyue.top

[R33] 捕获错误并提示行号
来源：http://irs.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ohj.shanyushiyangtech.top

[R34] 退出时清理
来源：http://mwx.jlsjyb.cn

trap 'rm -f "$tmp"' EXIT
来源：http://uxx.zhijiandao.cn

[R35] 后台执行并等待
来源：http://rrz.pengpengdd.cyou

sleep 5 & pid=$!; wait "$pid"
来源：http://che.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://yee.gzhubu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://sac.fehbvm.com

[R37] 把输出赋给变量
来源：http://ktr.guowangkeji.top

files=$(ls -1)
来源：http://rtn.yongpay.top

[R38] 管道串联
来源：http://xso.andypj.xyz

cat a.txt | grep -i error | wc -l
来源：http://mvi.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://wjz.zycfv.cn

cmd > out.log 2>&1
来源：http://oxi.yuanzhike.top

[R40] 追加写日志
来源：http://hbf.epnwcf.com

echo "log" >> out.log
来源：http://nas.jiagoushi.top

[R41] 丢弃输出
来源：http://dbn.fzhhl.top

cmd >/dev/null 2>&1
来源：http://zko.vqdsnc.cn

[R42] 输入重定向
来源：http://foz.tian-w.cn

wc -l < a.txt
来源：http://dfd.zhengqikj.top

[R43] 按名字查找文件
来源：http://esd.haohaochexian.top

find . -name "*.log" -type f
来源：http://rai.pycfn.com

[R44] 按修改时间查找
来源：http://fdb.jinqigufen.top

find . -mtime -7 -type f
来源：http://ttb.chenzaomai.com

[R45] 批量删除
来源：http://ufp.meibo888.top

find . -name "*.tmp" -delete
来源：http://uqk.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://vwq.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qwj.yj202588.top

[R47] sed 单行替换
来源：http://joj.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wtq.yvedp.cn

[R48] awk 取指定列
来源：http://did.jinyuanbaomall.cn

awk '{print $1, $3}' a.txt
来源：http://qjq.shuidangran.top

[R49] awk 带条件
来源：http://cqq.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qan.yj20258.top

[R50] awk 求和
来源：http://hwp.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://lyc.cashguo.top

[R51] 排序去重取前几
来源：http://fbi.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://smp.pengpengdd.cyou

[R52] 统计行数
来源：http://iep.hnqzz.top

wc -l a.txt
来源：http://lpz.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://phj.cqqwz.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://epx.uphjek.com

[R54] 比较两个文件
来源：http://vof.bbcook.cn

diff a.txt b.txt
来源：http://rre.ppjwa.cn

[R55] 压缩与解压
来源：http://rbn.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbe.cdnleiting.top

[R56] 远程拷贝
来源：http://hgi.epnwcf.com

scp file user@host:/path/
来源：http://jxs.cqqwz.cn

[R57] 远程执行命令
来源：http://nsj.fehbvm.com

ssh user@host 'uptime'
来源：http://gsr.ydzc1.top

[R58] 下载文件
来源：http://fbc.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kcs.epnwcf.com

[R59] 发 POST JSON
来源：http://exp.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hxk.pengpengdd.cyou

[R60] 只看 HTTP 状态码
来源：http://ljj.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uoc.shzxlz.cn

[R61] 磁盘占用
来源：http://jno.smart0.xyz


<!-- 参考信息 -->