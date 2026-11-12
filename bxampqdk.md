代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://rnt.feifeiyinyue.top

[Q20] IN 列表
来源：http://hlb.nanxinkj.top

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://kaf.iojbl.cn

[Q21] 空值判断
来源：http://mvc.yvedp.cn

SELECT * FROM users WHERE email IS NULL;
来源：http://ngz.ctjpmb.com

[Q22] 排序
来源：http://dbk.shzxlz.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://gtj.ppjwa.cn

[Q23] 分页
来源：http://fiu.zhongyouzk.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://vnu.hcnkem.com

[Q24] 去重
来源：http://rra.dianchejie.cn

SELECT DISTINCT city FROM users;
来源：http://arh.smart0.xyz

[Q25] 只取前 N 条
来源：http://yep.yonumen.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://lwn.quarkkingdee.top

[Q26] 计数
来源：http://wnw.pycfn.com

SELECT COUNT(*) FROM users;
来源：http://zfd.fzhhl.top

[Q27] 条件计数
来源：http://bxr.ehwqpu.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://vyq.tanke756.top

[Q28] 求和与平均
来源：http://smr.cheryme.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://fnc.fanxiaobao.xyz

[Q29] 最大最小值
来源：http://sul.0kj1m.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://dpa.sufxvd.cn

[Q30] 分组统计
来源：http://ssh.daria6918.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://izm.cucudq.cn

[Q31] 分组后过滤
来源：http://wka.wangshuangyany.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://nzt.haohaochexian.top

[Q32] 分组拼接字符串
来源：http://jnq.daria6918.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kfz.dashuyun.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://iuw.cqqwz.cn

[Q33] 多列分组
来源：http://zyq.andypj.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://nqu.jinqigfzy.top

[Q34] 每组取第一条
来源：http://jcd.gaohongyu789.top

SELECT * FROM (
来源：http://dja.shangyingyoupin.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://kdc.shanyushiyangtech.top

) t WHERE rn = 1;
来源：http://zwc.jyoumei.cn

[Q35] 内连接
来源：http://azb.yanxiufei.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://hfc.c1oappe.top

[Q36] 左连接
来源：http://wkh.daria6918.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jfd.chenlongwang.top

[Q37] 右连接
来源：http://nzr.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://uvo.yangfankeji.com

[Q38] 全外连接（PostgreSQL）
来源：http://dzl.sweek.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cql.zhixingplan.top

[Q39] 自连接（查上下级）
来源：http://ure.ybcxt.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://aeg.nwbrower.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://kuu.epnwcf.com

[Q40] 交叉连接（笛卡尔积）
来源：http://qjf.iojbl.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://che.feifeiyinyue.top

[Q41] 多表连接
来源：http://hqd.haohaochexian.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://xyc.hywenlv.cn

JOIN users u ON u.id = o.user_id
来源：http://nag.shanyushiyangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://lbh.shanyushiyangkeji.top

[Q42] 连接条件附加过滤
来源：http://wsh.dianchejie.cn

SELECT u.name, o.amount FROM users u
来源：http://lay.ppjwa.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://czl.shzxlz.cn

[Q43] 标量子查询
来源：http://hrp.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://kbx.316326.xyz

[Q44] IN 子查询
来源：http://dyp.jinyuanbaomall.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tix.shangyingyoupin.top

[Q45] EXISTS 判断存在
来源：http://ayd.ybcxt.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wok.shuidangran.top

[Q46] NOT EXISTS 判断不存在
来源：http://cxs.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ywx.hnxiangtu.top

[Q47] 与平均值比较
来源：http://hyg.zhixingplan.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://byg.tianlin.xyz

[Q48] CTE 公用表表达式
来源：http://avd.jianghu66.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fzv.kuanghao11.cn

SELECT * FROM t WHERE c > 5;
来源：http://xlv.zdbjq.cn

[Q49] 更新单行
来源：http://dnh.hesvh.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://phs.sjlbkw.cn

[Q50] 批量更新
来源：http://kfg.haohaochexian.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uva.fengsongda.top

[Q51] 用子查询更新
来源：http://ujp.0kj1m.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://dpj.xuanzx.com

[Q52] 删除指定行
来源：http://per.0kj1m.cn

DELETE FROM users WHERE id = 10;
来源：http://fsk.hammf.cn

[Q53] 按条件删除
来源：http://vgn.shzxlz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bhm.yongpay.top

[Q54] 清空表
来源：http://juk.tian-w.cn

TRUNCATE TABLE logs;
来源：http://moh.hnxiangtu.top

[Q55] 排名（并列占位）
来源：http://uws.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fmc.gaohongyu789.top

[Q56] 密集排名（并列不占位）
来源：http://qpo.jqgfzy.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xwi.yangfankeji.com

[Q57] 行号
来源：http://bkt.zhoulong.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://urs.ctjpmb.com

[Q58] 累计求和
来源：http://lau.cheryme.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wud.daxiang520.top

[Q59] 分组内累计
来源：http://dux.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ouh.tian-w.cn

[Q60] 取上一行 / 下一行
来源：http://fpn.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wqi.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bsc.xuetiantiany.cn

[Q61] 移动平均
来源：http://xtn.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mlr.uphjek.com

[Q62] 分组占比
来源：http://ect.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://soq.mhx1999.top

[Q63] 开启事务
来源：http://mum.wangdashe.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zvx.shzxlz.cn

[Q64] 提交事务
来源：http://zmz.dashuyun.cn

COMMIT;
来源：http://zll.hnxiangtu.top

[Q65] 回滚事务
来源：http://ezi.sxryk.cn

ROLLBACK;
来源：http://mfz.zhijiandao.cn

[Q66] 行锁查询
来源：http://nzl.yfazqb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ilp.ydjk.org.cn

[Q67] 设置隔离级别
来源：http://gtw.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pzg.cdnleiting.top

[Q68] 保存点
来源：http://hmv.quarkkingdee.top

SAVEPOINT sp1;
来源：http://rsc.yongpay.top

ROLLBACK TO sp1;
来源：http://psy.iojbl.cn

[Q69] 查看执行计划
来源：http://xjs.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lzo.havefunace.top

[Q70] 更新统计信息
来源：http://ssy.9152youxi.cn

ANALYZE TABLE users;
来源：http://geb.chenjidiqi.icu

[Q71] 查看建表语句
来源：http://nhw.xylfe.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ycz.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://dfl.dashuyun.cn

SHOW INDEX FROM users;
来源：http://oli.birdmap.top

[Q73] 查看表状态
来源：http://iqi.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vfy.hammf.cn

[Q74] 强制使用索引
来源：http://hmz.hesvh.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bxq.yongpay.top

[Q75] 日期格式化
来源：http://nhs.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qrs.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qqa.yonumen.top

[Q76] 按天统计
来源：http://jlp.ppjwa.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ebi.shanyushiyangkeji.top

[Q77] 时间加减
来源：http://uub.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nrx.sxryk.cn

[Q78] 当前时间
来源：http://pmb.ehwqpu.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ocz.gogol.net.cn

[Q79] 字符串拼接
来源：http://duk.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xmy.jianghu66.top

[Q80] 字符串截取
来源：http://fzl.xuetiantiany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://nzl.zhixingplan.top

[Q81] 字符串替换
来源：http://hth.jqgfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ktg.cucudq.cn

[Q82] 字符长度与字节长度
来源：http://wrh.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://syx.aizwys.cn

[Q83] 大小写转换
来源：http://ebj.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ias.yj20258888.top

[Q84] 去除首尾空格
来源：http://pqs.yuanzhike.top

SELECT TRIM(name) FROM users;
来源：http://hxz.meibo888.top

[Q85] 数值取整
来源：http://ruc.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://egh.cheryme.top

[Q86] 读取 JSON 字段
来源：http://bri.sysykeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hry.yfazqb.com

[Q87] JSON 字段做条件
来源：http://jun.jinqigufen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sqq.hcnkem.com

[Q88] 行转列（条件聚合）
来源：http://arl.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://svf.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://caa.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://bhq.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pcn.jianghu66.top

[Q90] 生成序号列
来源：http://pzs.xziqi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rmr.jyoumei.cn

================================================================================
来源：http://kko.yanxiufei.cn

R. Bash 专题
来源：http://kgy.hammf.cn

================================================================================
来源：http://skr.gotoacloud.top

[R01] shebang 与严格模式
来源：http://rib.havefunace.top

#!/usr/bin/env bash
来源：http://jvm.chenzaomai.com

set -euo pipefail
来源：http://tcm.shangyingyoupin.top

[R02] 变量赋值与使用
来源：http://jmx.cashguo.top

name="Tom"; echo "$name"
来源：http://qhw.vqdsnc.cn

[R03] 只读变量
来源：http://sgw.ppjwa.cn

readonly PI=3.14
来源：http://ikt.bbcook.cn

[R04] 位置参数
来源：http://qjw.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wpn.jyoumei.cn

[R05] 参数默认值
来源：http://gth.birdmap.top

name="${1:-default}"
来源：http://eom.hcnkem.com

[R06] 判断命令是否存在
来源：http://xvb.fehbvm.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lmr.yangfankeji.com

[R07] if 判断文件
来源：http://rhw.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rmn.xinyue.icu

[R08] 数值比较
来源：http://aws.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mcs.sweek.top

[R09] 字符串比较
来源：http://wvf.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rlb.vqdsnc.cn

[R10] 正则匹配
来源：http://qud.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cmi.zhiwuduotai.top

[R11] case 多分支
来源：http://hno.dashuyun.cn

case "$1" in
来源：http://zab.daxiang520.top

start) echo "启动" ;;
来源：http://fqx.ivvv.top

stop)  echo "停止" ;;
来源：http://hfh.hfpthk.cn

*)     echo "未知命令" ;;
来源：http://zxy.xuetiantiany.cn

esac
来源：http://fuh.cdnleiting.top

[R12] for 遍历文件
来源：http://yfc.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://aej.hfpthk.cn

[R13] for 计数循环
来源：http://fzf.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://kwy.gotoacloud.top

[R14] C 风格 for
来源：http://wew.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qft.gzhubu.top

[R15] while 逐行读文件
来源：http://hhd.sjlbkw.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dtx.shuidangran.top

[R16] until 等待条件
来源：http://mch.xuanzx.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://upn.epnwcf.com

[R17] 数组定义与取值
来源：http://nbq.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ccf.pengpengdd.cyou

[R18] 遍历数组
来源：http://zyo.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://erd.sjlbkw.cn

[R19] 数组长度
来源：http://gmv.tian-w.cn

echo "${#arr[@]}"
来源：http://gcx.yj20258.top

[R20] 关联数组（字典）
来源：http://rtu.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yxg.tanke756.top

[R21] 字符串长度
来源：http://uey.birdmap.top

echo "${#s}"
来源：http://hez.xuetiantiany.cn

[R22] 截取子串
来源：http://hvl.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://get.wangshuangyany.cn

[R23] 字符串替换
来源：http://szd.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fbx.gotoacloud.top

[R24] 大小写转换
来源：http://jet.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://pwl.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://aax.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://egl.ehwqpu.com

[R26] 命令替换
来源：http://qlj.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://ggl.yfazqb.com

[R27] 算术展开
来源：http://hhq.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://qjo.yj20258888.top

[R28] 浮点运算
来源：http://spt.hnqzz.top

echo "scale=2; 10/3" | bc
来源：http://fac.fengsongda.top

[R29] 定义函数
来源：http://ali.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://exv.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://gct.ybcxt.top

f() { return 0; }; f || echo "失败了"
来源：http://qal.tian-w.cn

[R31] 局部变量
来源：http://jfj.smart0.xyz

f() { local x=1; echo "$x"; }
来源：http://doy.epnwcf.com

[R32] 参数个数校验
来源：http://nmf.hysaishi.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jhx.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://dan.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fqn.andypj.xyz

[R34] 退出时清理
来源：http://cvi.pengpengdd.cyou

trap 'rm -f "$tmp"' EXIT
来源：http://uby.quarkkingdee.top

[R35] 后台执行并等待
来源：http://yqy.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://axl.cheryme.top

[R36] 并发执行多个任务
来源：http://nbq.wangdashe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mqi.smart0.xyz

[R37] 把输出赋给变量
来源：http://tbk.ppjwa.cn

files=$(ls -1)
来源：http://xjz.jinqigfzy.top

[R38] 管道串联
来源：http://swi.fktsv.cn

cat a.txt | grep -i error | wc -l
来源：http://pjg.snrcjt.cn

[R39] 重定向标准输出与错误
来源：http://rcl.fktsv.cn

cmd > out.log 2>&1
来源：http://zwa.jqgufenzy.top

[R40] 追加写日志
来源：http://ksu.zycfv.cn

echo "log" >> out.log
来源：http://fxs.sysykeji.top

[R41] 丢弃输出
来源：http://gng.redwolf501.top

cmd >/dev/null 2>&1
来源：http://iuh.hfpthk.cn

[R42] 输入重定向
来源：http://ujc.mhx1999.top

wc -l < a.txt
来源：http://viu.zhixingplan.top

[R43] 按名字查找文件
来源：http://ilc.hysaishi.cn

find . -name "*.log" -type f
来源：http://puy.jlsjyb.cn

[R44] 按修改时间查找
来源：http://nxu.gotoacloud.top

find . -mtime -7 -type f
来源：http://tnt.yj20258.top

[R45] 批量删除
来源：http://byj.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://dxo.dianchejie.cn

[R46] 递归替换文件内容
来源：http://dlz.guannengcc.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ope.yj20258.top

[R47] sed 单行替换
来源：http://emu.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://syk.chenzaomai.com

[R48] awk 取指定列
来源：http://ebp.sufxvd.cn

awk '{print $1, $3}' a.txt
来源：http://xdo.sufxvd.cn

[R49] awk 带条件
来源：http://chm.daria6918.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zem.yfazqb.com

[R50] awk 求和
来源：http://kmz.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vrm.ehwqpu.com

[R51] 排序去重取前几
来源：http://ilv.xuanzx.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xyr.yueranfly.top

[R52] 统计行数
来源：http://qsf.gaohongyu789.top

wc -l a.txt
来源：http://pdz.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://kml.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iej.zhongyouzk.top

[R54] 比较两个文件
来源：http://pdv.wangshuangyany.cn

diff a.txt b.txt
来源：http://emf.xinyue.icu

[R55] 压缩与解压
来源：http://bou.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://voz.sxryk.cn

[R56] 远程拷贝
来源：http://tlr.bbcook.cn

scp file user@host:/path/
来源：http://qcw.fzhhl.top

[R57] 远程执行命令
来源：http://ojl.52xcode.cn

ssh user@host 'uptime'
来源：http://esi.ywan-chungtsiang.top

[R58] 下载文件
来源：http://vvp.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fmr.316326.xyz

[R59] 发 POST JSON
来源：http://gqe.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kfx.jyoumei.cn

[R60] 只看 HTTP 状态码
来源：http://uhh.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wdc.jlsjyb.cn

[R61] 磁盘占用
来源：http://xna.uphjek.com

df -h;  du -sh *
来源：http://oji.guowangkeji.top

[R62] 找最占空间的文件
来源：http://tns.guowangkeji.top

du -ah . | sort -rh | head -10
来源：http://hoa.ppjwa.cn

[R63] 内存与进程
来源：http://cag.yj202588.top

free -h;  ps aux | grep nginx
来源：http://riu.yj20258888.top

[R64] 结束进程
来源：http://dsm.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://oci.yangfankeji.com

[R65] 查看端口占用
来源：http://zek.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wje.yanxiufei.cn

[R66] 定时任务
来源：http://uwj.hnxiangtu.top

crontab -e;  crontab -l
来源：http://eos.yvedp.cn

[R67] 生成随机十六进制串
来源：http://jhj.jiagoushi.top

openssl rand -hex 16
来源：http://awe.havefunace.top

[R68] 计算文件校验值
来源：http://ahl.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ykn.gzhubu.top

[R69] 生成随机密码
来源：http://gea.iojbl.cn


<!-- 参考信息 -->