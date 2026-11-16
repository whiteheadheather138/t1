代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://vel.jqgfzy.top

[Q18] 模糊匹配
来源：http://jma.vehdjk.com

SELECT * FROM users WHERE name LIKE '张%';
来源：http://bjj.wangdashe.top

[Q19] 范围查询
来源：http://xte.yongpay.top

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://sdu.fktsv.cn

[Q20] IN 列表
来源：http://zci.hysaishi.cn

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://pkz.wangdashe.top

[Q21] 空值判断
来源：http://uyw.shangyingyoupin.top

SELECT * FROM users WHERE email IS NULL;
来源：http://txk.tarul.cn

[Q22] 排序
来源：http://hdx.zhongyouzk.top

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://dgz.quarkkingdee.top

[Q23] 分页
来源：http://pai.zhijiandao.cn

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mrg.fanxiaobao.xyz

[Q24] 去重
来源：http://egl.fehbvm.com

SELECT DISTINCT city FROM users;
来源：http://erd.jinyuanbaomall.cn

[Q25] 只取前 N 条
来源：http://pob.jinqigfzy.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wng.tianlin.xyz

[Q26] 计数
来源：http://bxe.svipenyu.cn

SELECT COUNT(*) FROM users;
来源：http://con.ybcxt.top

[Q27] 条件计数
来源：http://qlw.ydjk.org.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://bel.jqgfzy.top

[Q28] 求和与平均
来源：http://ibi.xylfe.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://bld.316326.xyz

[Q29] 最大最小值
来源：http://oiy.zycfv.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://pip.jyoumei.cn

[Q30] 分组统计
来源：http://nte.0kj1m.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://rxe.zhengqikj.top

[Q31] 分组后过滤
来源：http://aqx.jinqigufen.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://voi.zhoulong.xyz

[Q32] 分组拼接字符串
来源：http://mgq.cheryme.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://upc.aizwys.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://ulh.smart0.xyz

[Q33] 多列分组
来源：http://mdu.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ocf.cdnleiting.top

[Q34] 每组取第一条
来源：http://dcq.dashuyun.cn

SELECT * FROM (
来源：http://omy.epnwcf.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://auq.yj20258888.top

) t WHERE rn = 1;
来源：http://vcb.yangfankeji.com

[Q35] 内连接
来源：http://tqj.hywenlv.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://xha.guannengcc.top

[Q36] 左连接
来源：http://zkp.chenjidiqi.icu

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://tkc.yuxming.cn

[Q37] 右连接
来源：http://cxr.shangyingyoupin.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lpw.chenzaomai.com

[Q38] 全外连接（PostgreSQL）
来源：http://tfn.jlsjyb.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qme.fengsongda.top

[Q39] 自连接（查上下级）
来源：http://mss.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://lnf.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pvi.yfazqb.com

[Q40] 交叉连接（笛卡尔积）
来源：http://okw.havefunace.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hfg.havefunace.top

[Q41] 多表连接
来源：http://xqe.zhaomingkeji.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://air.0kj1m.cn

JOIN users u ON u.id = o.user_id
来源：http://bhf.xinyue.icu

JOIN products p ON p.id = o.product_id;
来源：http://qhy.yangfankeji.com

[Q42] 连接条件附加过滤
来源：http://lbk.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://dov.xziqi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://tmv.jinqigfzy.top

[Q43] 标量子查询
来源：http://abn.fehbvm.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wbp.smart0.xyz

[Q44] IN 子查询
来源：http://kuw.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://dcc.jianghu66.top

[Q45] EXISTS 判断存在
来源：http://pwd.snrcjt.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://tlz.zhoulong.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://xur.shangyingyoupin.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ydb.bjfxy.top

[Q47] 与平均值比较
来源：http://iud.cheryme.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dkd.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://oyd.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wco.zhiwuduotai.top

SELECT * FROM t WHERE c > 5;
来源：http://abc.fengsongda.top

[Q49] 更新单行
来源：http://zad.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xvi.yvedp.cn

[Q50] 批量更新
来源：http://twu.yanxiufei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lkr.sweek.top

[Q51] 用子查询更新
来源：http://sbv.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kfz.jiagoushi.top

[Q52] 删除指定行
来源：http://znp.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://hzg.yvedp.cn

[Q53] 按条件删除
来源：http://cpy.chenlongwang.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hfo.zhaomingkeji.xyz

[Q54] 清空表
来源：http://oti.yuanzhike.top

TRUNCATE TABLE logs;
来源：http://bgy.haohaochexian.top

[Q55] 排名（并列占位）
来源：http://ibw.fktsv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mqy.cqqwz.cn

[Q56] 密集排名（并列不占位）
来源：http://ktw.pycfn.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uqg.vehdjk.com

[Q57] 行号
来源：http://cry.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sco.zycfv.cn

[Q58] 累计求和
来源：http://lie.chenzaomai.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nvo.xuetiantiany.cn

[Q59] 分组内累计
来源：http://ibu.jinyuanbaomall.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://cej.zhengqikj.top

[Q60] 取上一行 / 下一行
来源：http://kxx.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://lfy.vqdsnc.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hxe.daria6918.cn

[Q61] 移动平均
来源：http://pdr.hnxiangtu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://syi.wangshuangyany.cn

[Q62] 分组占比
来源：http://jgr.tarul.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://pvf.pengpengdd.cyou

[Q63] 开启事务
来源：http://shw.shangyingyoupin.top

START TRANSACTION;                -- 或 BEGIN
来源：http://sce.xziqi.cn

[Q64] 提交事务
来源：http://prm.birdmap.top

COMMIT;
来源：http://cqk.shanyushiyangkeji.top

[Q65] 回滚事务
来源：http://tdg.zhoulong.xyz

ROLLBACK;
来源：http://fvt.gogol.net.cn

[Q66] 行锁查询
来源：http://rza.quarkkingdee.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eoo.meibo888.top

[Q67] 设置隔离级别
来源：http://asn.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iur.nanxinkj.top

[Q68] 保存点
来源：http://cwf.daxiang520.top

SAVEPOINT sp1;
来源：http://dyg.316326.xyz

ROLLBACK TO sp1;
来源：http://ebv.ehwqpu.com

[Q69] 查看执行计划
来源：http://veq.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eex.chenlongwang.top

[Q70] 更新统计信息
来源：http://kpq.vehdjk.com

ANALYZE TABLE users;
来源：http://swj.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://bap.xingfuxueyuan.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iic.yfazqb.com

[Q72] 查看索引
来源：http://cyr.zdqjudy.top

SHOW INDEX FROM users;
来源：http://yqn.0kj1m.cn

[Q73] 查看表状态
来源：http://ucw.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://nvz.hesvh.cn

[Q74] 强制使用索引
来源：http://qzn.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zay.cucudq.cn

[Q75] 日期格式化
来源：http://jxm.0kj1m.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pns.zycfv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vtx.jyoumei.cn

[Q76] 按天统计
来源：http://goy.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jfg.pycfn.com

[Q77] 时间加减
来源：http://vcz.guannengcc.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cdk.zdqjudy.top

[Q78] 当前时间
来源：http://hrz.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jvb.shzxlz.cn

[Q79] 字符串拼接
来源：http://eiw.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uwt.chenlongwang.top

[Q80] 字符串截取
来源：http://zkn.cqqwz.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rkk.52xcode.cn

[Q81] 字符串替换
来源：http://diw.quarkkingdee.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://akf.nwbrower.top

[Q82] 字符长度与字节长度
来源：http://wid.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://boj.snrcjt.cn

[Q83] 大小写转换
来源：http://krz.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fxs.cheryme.top

[Q84] 去除首尾空格
来源：http://gan.snrcjt.cn

SELECT TRIM(name) FROM users;
来源：http://hua.hywenlv.cn

[Q85] 数值取整
来源：http://ufl.xuetiantiany.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://eng.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://rhd.gaohongyu789.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nqd.yvedp.cn

[Q87] JSON 字段做条件
来源：http://snq.jinyuanbaomall.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hki.xuetiantiany.cn

[Q88] 行转列（条件聚合）
来源：http://cmx.tian-w.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ngl.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dma.havefunace.top

[Q89] 判断表是否存在
来源：http://tvs.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qtg.guannengcc.top

[Q90] 生成序号列
来源：http://ndd.c1oappe.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qoi.yuxming.cn

================================================================================
来源：http://rfg.dianchejie.cn

R. Bash 专题
来源：http://sbs.hysaishi.cn

================================================================================
来源：http://giz.yj20258.top

[R01] shebang 与严格模式
来源：http://cpy.tian-w.cn

#!/usr/bin/env bash
来源：http://uqk.fktsv.cn

set -euo pipefail
来源：http://aso.mhx1999.top

[R02] 变量赋值与使用
来源：http://sfc.dianchejie.cn

name="Tom"; echo "$name"
来源：http://yop.yvedp.cn

[R03] 只读变量
来源：http://plo.meibo888.top

readonly PI=3.14
来源：http://ago.xinyue.icu

[R04] 位置参数
来源：http://zfz.hcnkem.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fav.sufxvd.cn

[R05] 参数默认值
来源：http://sxt.hongshengwenyu.top

name="${1:-default}"
来源：http://hbb.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://wwx.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qgw.meibo888.top

[R07] if 判断文件
来源：http://qkw.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://iqy.chenzaomai.com

[R08] 数值比较
来源：http://xdt.jinqigufen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ksn.yongpay.top

[R09] 字符串比较
来源：http://tmk.hongshengwenyu.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mfx.birdmap.top

[R10] 正则匹配
来源：http://lnt.hammf.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jyf.ehwqpu.com

[R11] case 多分支
来源：http://mbk.cashguo.top

case "$1" in
来源：http://yfx.daria6918.cn

start) echo "启动" ;;
来源：http://ipj.smart0.xyz

stop)  echo "停止" ;;
来源：http://xac.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://pdy.yj20258888.top

esac
来源：http://xrt.dianchejie.cn

[R12] for 遍历文件
来源：http://app.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://iiy.shuidangran.top

[R13] for 计数循环
来源：http://tbu.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://sro.yvedp.cn

[R14] C 风格 for
来源：http://pfb.jyoumei.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iue.fengsongda.top

[R15] while 逐行读文件
来源：http://sof.jqgufenzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jtt.cucudq.cn

[R16] until 等待条件
来源：http://ydk.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rdy.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://pqw.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://fsb.guowangkeji.top

[R18] 遍历数组
来源：http://mih.nanxuanxn.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pnp.vehdjk.com

[R19] 数组长度
来源：http://mud.smart0.xyz

echo "${#arr[@]}"
来源：http://spw.zdqjudy.top

[R20] 关联数组（字典）
来源：http://cec.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lxd.ctjpmb.com

[R21] 字符串长度
来源：http://osn.snrcjt.cn

echo "${#s}"
来源：http://ndr.jiagoushi.top

[R22] 截取子串
来源：http://pog.chenzaomai.com

echo "${s:0:5}"
来源：http://uvd.sweek.top

[R23] 字符串替换
来源：http://sgg.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cyd.cdnleiting.top

[R24] 大小写转换
来源：http://pcw.chenjidiqi.icu

echo "${s^^}"; echo "${s,,}"
来源：http://azk.sysykeji.top

[R25] 去后缀 / 去前缀
来源：http://gcc.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://tmj.jqgfzy.top

[R26] 命令替换
来源：http://vtd.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://dsl.epnwcf.com

[R27] 算术展开
来源：http://qsr.bjfxy.top

echo $((1 + 2 * 3))
来源：http://wsv.9152youxi.cn

[R28] 浮点运算
来源：http://ojz.cheryme.top

echo "scale=2; 10/3" | bc
来源：http://vhh.fktsv.cn

[R29] 定义函数
来源：http://zub.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ufo.zhixingplan.top

[R30] 函数返回状态码
来源：http://mfl.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://fuj.yangfankeji.com

[R31] 局部变量
来源：http://jkv.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://jcp.pengpengdd.cyou

[R32] 参数个数校验
来源：http://rwr.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qwo.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://gvn.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yfz.nwbrower.top

[R34] 退出时清理
来源：http://kfa.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://dyh.c1oappe.top

[R35] 后台执行并等待
来源：http://fcx.fehbvm.com

sleep 5 & pid=$!; wait "$pid"
来源：http://iaq.sweek.top

[R36] 并发执行多个任务
来源：http://onn.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vhv.52xcode.cn

[R37] 把输出赋给变量
来源：http://yzl.sxryk.cn

files=$(ls -1)
来源：http://rtt.yj20258.top

[R38] 管道串联
来源：http://cmq.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://hjm.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://aex.hammf.cn

cmd > out.log 2>&1
来源：http://xab.nanxuanxn.top

[R40] 追加写日志
来源：http://jgg.quarkkingdee.top

echo "log" >> out.log
来源：http://zef.xuanzx.com

[R41] 丢弃输出
来源：http://aev.pycfn.com

cmd >/dev/null 2>&1
来源：http://uxk.cdnleiting.top

[R42] 输入重定向
来源：http://jxq.52xcode.cn

wc -l < a.txt
来源：http://pda.haohaochexian.top

[R43] 按名字查找文件
来源：http://fds.wangdashe.top

find . -name "*.log" -type f
来源：http://dyw.jianghu66.top

[R44] 按修改时间查找
来源：http://mzw.yanxiufei.cn

find . -mtime -7 -type f
来源：http://orb.yj202588.top

[R45] 批量删除
来源：http://imo.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://qgy.shuidangran.top

[R46] 递归替换文件内容
来源：http://kyi.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://knl.sysykeji.top

[R47] sed 单行替换
来源：http://nek.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://fmz.meibo888.top

[R48] awk 取指定列
来源：http://fjc.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://ezn.jinghuilouyu.cn

[R49] awk 带条件
来源：http://lsf.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zdc.sjlbkw.cn

[R50] awk 求和
来源：http://hju.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sbt.shanyushiyangtech.top

[R51] 排序去重取前几
来源：http://omf.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ufc.dianchejie.cn

[R52] 统计行数
来源：http://hbu.sweek.top

wc -l a.txt
来源：http://ixe.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://duz.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jzg.dashuyun.cn

[R54] 比较两个文件
来源：http://uau.hcnkem.com

diff a.txt b.txt
来源：http://bsk.shuidangran.top

[R55] 压缩与解压
来源：http://uat.yanxiufei.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sak.bjfxy.top

[R56] 远程拷贝
来源：http://wgh.jyoumei.cn

scp file user@host:/path/
来源：http://rst.52xcode.cn

[R57] 远程执行命令
来源：http://bka.yangfankeji.com

ssh user@host 'uptime'
来源：http://pxz.nanxinkj.top

[R58] 下载文件
来源：http://bxf.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pgf.zhoulong.xyz

[R59] 发 POST JSON
来源：http://hpm.snrcjt.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vic.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://bgd.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vdc.gotoacloud.top

[R61] 磁盘占用
来源：http://bbn.yangfankeji.com

df -h;  du -sh *
来源：http://ujj.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://ddd.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://qbp.hysaishi.cn

[R63] 内存与进程
来源：http://wyv.shangyingyoupin.top

free -h;  ps aux | grep nginx
来源：http://onw.gotoacloud.top

[R64] 结束进程
来源：http://dbi.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://vna.yongpay.top

[R65] 查看端口占用
来源：http://svc.hnqzz.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ino.sufxvd.cn

[R66] 定时任务
来源：http://kzz.zycfv.cn

crontab -e;  crontab -l
来源：http://ahi.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://efe.yongpay.top


<!-- 参考信息 -->