代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://xyv.zhongyouzk.top

[Q20] IN 列表
来源：http://bsl.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://zfx.jinyuanbaomall.cn

[Q21] 空值判断
来源：http://zxr.shanyushiyangtech.top

SELECT * FROM users WHERE email IS NULL;
来源：http://ylb.shangyingyoupin.top

[Q22] 排序
来源：http://vaw.pycfn.com

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mqv.havefunace.top

[Q23] 分页
来源：http://ala.cdnleiting.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://dvd.yj20258.top

[Q24] 去重
来源：http://cpl.wangshuangyany.cn

SELECT DISTINCT city FROM users;
来源：http://rtm.svipenyu.cn

[Q25] 只取前 N 条
来源：http://fse.hesvh.cn

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ttm.tian-w.cn

[Q26] 计数
来源：http://xal.cucudq.cn

SELECT COUNT(*) FROM users;
来源：http://cxr.hesvh.cn

[Q27] 条件计数
来源：http://yzd.tarul.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://zrl.vehdjk.com

[Q28] 求和与平均
来源：http://jzj.yuxming.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://dhm.xingfuxueyuan.xyz

[Q29] 最大最小值
来源：http://ktm.jinqigfzy.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://pqt.hesvh.cn

[Q30] 分组统计
来源：http://vzd.9152youxi.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ywc.andypj.xyz

[Q31] 分组后过滤
来源：http://kto.jinyuanbaomall.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://jqm.pycfn.com

[Q32] 分组拼接字符串
来源：http://zjd.feifeiyinyue.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jkf.andypj.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://qha.zhoulong.xyz

[Q33] 多列分组
来源：http://jfn.gotoacloud.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://oha.jinyuanbaomall.cn

[Q34] 每组取第一条
来源：http://lez.sysykeji.top

SELECT * FROM (
来源：http://zir.hfpthk.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://gnu.wangdashe.top

) t WHERE rn = 1;
来源：http://xmc.hcnkem.com

[Q35] 内连接
来源：http://tec.havefunace.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://nqh.jyoumei.cn

[Q36] 左连接
来源：http://tzq.zycfv.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://jsh.vehdjk.com

[Q37] 右连接
来源：http://crw.jinghuilouyu.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ehf.sxryk.cn

[Q38] 全外连接（PostgreSQL）
来源：http://qdv.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dvj.dianchejie.cn

[Q39] 自连接（查上下级）
来源：http://hli.xylfe.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://huw.xziqi.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://neu.pengpengdd.cyou

[Q40] 交叉连接（笛卡尔积）
来源：http://kkq.guowangkeji.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rer.zhijiandao.cn

[Q41] 多表连接
来源：http://xpd.yj20258.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://uly.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://ynf.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://mqx.zhengqikj.top

[Q42] 连接条件附加过滤
来源：http://hqs.havefunace.top

SELECT u.name, o.amount FROM users u
来源：http://zjd.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fne.havefunace.top

[Q43] 标量子查询
来源：http://coq.aibaodan.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://itt.zdqjudy.top

[Q44] IN 子查询
来源：http://kgo.redwolf501.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://cgx.chenjidiqi.icu

[Q45] EXISTS 判断存在
来源：http://uvd.52xcode.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bxs.zycfv.cn

[Q46] NOT EXISTS 判断不存在
来源：http://niq.ctjpmb.com

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rid.jinqigfzy.top

[Q47] 与平均值比较
来源：http://qpu.yuxming.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://zgm.zhijiandao.cn

[Q48] CTE 公用表表达式
来源：http://jwk.gzhubu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqf.fktsv.cn

SELECT * FROM t WHERE c > 5;
来源：http://xes.svipenyu.cn

[Q49] 更新单行
来源：http://qqn.pengpengdd.cyou

UPDATE users SET status = 1 WHERE id = 10;
来源：http://juf.tianlin.xyz

[Q50] 批量更新
来源：http://gvy.hywenlv.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lqt.meibo888.top

[Q51] 用子查询更新
来源：http://iwr.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hhb.hfpthk.cn

[Q52] 删除指定行
来源：http://osw.iojbl.cn

DELETE FROM users WHERE id = 10;
来源：http://yty.yanxiufei.cn

[Q53] 按条件删除
来源：http://xrv.nanxinkj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zzu.wangdashe.top

[Q54] 清空表
来源：http://vfx.hnqzz.top

TRUNCATE TABLE logs;
来源：http://ohj.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://gog.gzhubu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ozk.yanxiufei.cn

[Q56] 密集排名（并列不占位）
来源：http://hxo.chenzaomai.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://kvm.feifeiyinyue.top

[Q57] 行号
来源：http://inn.yj20258.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lru.shzxlz.cn

[Q58] 累计求和
来源：http://hgu.shanyushiyangkeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dfq.aizwys.cn

[Q59] 分组内累计
来源：http://ddb.yanxiufei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wnf.hywenlv.cn

[Q60] 取上一行 / 下一行
来源：http://yss.yj202588.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fic.yj20258.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rfu.xylfe.cn

[Q61] 移动平均
来源：http://liy.ppjwa.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://rwl.svipenyu.cn

[Q62] 分组占比
来源：http://xuu.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eji.daria6918.cn

[Q63] 开启事务
来源：http://pwa.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://yyg.hcnkem.com

[Q64] 提交事务
来源：http://uhx.sweek.top

COMMIT;
来源：http://bly.vehdjk.com

[Q65] 回滚事务
来源：http://oyz.ppjwa.cn

ROLLBACK;
来源：http://hrp.shzxlz.cn

[Q66] 行锁查询
来源：http://exl.chenzaomai.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://spd.jinqigfzy.top

[Q67] 设置隔离级别
来源：http://vok.ivvv.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ebp.gaohongyu789.top

[Q68] 保存点
来源：http://hjx.ehwqpu.com

SAVEPOINT sp1;
来源：http://qug.jianghu66.top

ROLLBACK TO sp1;
来源：http://jdw.zycfv.cn

[Q69] 查看执行计划
来源：http://xnl.gotoacloud.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nao.yanxiufei.cn

[Q70] 更新统计信息
来源：http://ggc.gogol.net.cn

ANALYZE TABLE users;
来源：http://ydo.fehbvm.com

[Q71] 查看建表语句
来源：http://mkc.zhixingplan.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mbc.gzhubu.top

[Q72] 查看索引
来源：http://fld.haohaochexian.top

SHOW INDEX FROM users;
来源：http://hwf.zhengqikj.top

[Q73] 查看表状态
来源：http://gmi.havefunace.top

SHOW TABLE STATUS LIKE 'users';
来源：http://uur.snrcjt.cn

[Q74] 强制使用索引
来源：http://rgu.uphjek.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://vff.hysaishi.cn

[Q75] 日期格式化
来源：http://ztl.ivvv.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kuf.cashguo.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rsb.ybcxt.top

[Q76] 按天统计
来源：http://qjd.cqqwz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fvh.jlsjyb.cn

[Q77] 时间加减
来源：http://nqr.tanke756.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ysi.jianghu66.top

[Q78] 当前时间
来源：http://sme.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gta.fehbvm.com

[Q79] 字符串拼接
来源：http://tjr.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ika.hcnkem.com

[Q80] 字符串截取
来源：http://vud.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hdl.hesvh.cn

[Q81] 字符串替换
来源：http://qju.hnxiangtu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pia.smart0.xyz

[Q82] 字符长度与字节长度
来源：http://zno.dashuyun.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gnk.ybcxt.top

[Q83] 大小写转换
来源：http://zha.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ubh.zhaomingkeji.xyz

[Q84] 去除首尾空格
来源：http://ipi.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://xxk.wangshuangyany.cn

[Q85] 数值取整
来源：http://jmt.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hqm.316326.xyz

[Q86] 读取 JSON 字段
来源：http://lus.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zgj.cqqwz.cn

[Q87] JSON 字段做条件
来源：http://hsg.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vyc.aibaodan.cn

[Q88] 行转列（条件聚合）
来源：http://eeu.fktsv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ugi.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bdl.zdbjq.cn

[Q89] 判断表是否存在
来源：http://loa.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rft.pengpengdd.cyou

[Q90] 生成序号列
来源：http://mxk.daxiang520.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xcd.daxiang520.top

================================================================================
来源：http://emj.jyoumei.cn

R. Bash 专题
来源：http://stf.andypj.xyz

================================================================================
来源：http://wkc.xingfuxueyuan.xyz

[R01] shebang 与严格模式
来源：http://xft.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://pxk.shzxlz.cn

set -euo pipefail
来源：http://ibx.zdqjudy.top

[R02] 变量赋值与使用
来源：http://dwp.sysykeji.top

name="Tom"; echo "$name"
来源：http://yvg.sjlbkw.cn

[R03] 只读变量
来源：http://xjg.cheryme.top

readonly PI=3.14
来源：http://zce.chenjidiqi.icu

[R04] 位置参数
来源：http://kxo.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xyh.mhx1999.top

[R05] 参数默认值
来源：http://mmm.zhaomingkeji.xyz

name="${1:-default}"
来源：http://cym.fehbvm.com

[R06] 判断命令是否存在
来源：http://anm.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sqj.cashguo.top

[R07] if 判断文件
来源：http://ziw.hysaishi.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://viy.cashguo.top

[R08] 数值比较
来源：http://itr.yonumen.top

if (( a > b )); then echo "a 更大"; fi
来源：http://etq.zycfv.cn

[R09] 字符串比较
来源：http://neg.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yci.jlsjyb.cn

[R10] 正则匹配
来源：http://dof.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bfs.9152youxi.cn

[R11] case 多分支
来源：http://nmq.quarkkingdee.top

case "$1" in
来源：http://kcy.jqgfzy.top

start) echo "启动" ;;
来源：http://wbe.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://cwh.snrcjt.cn

*)     echo "未知命令" ;;
来源：http://fyl.yuxming.cn

esac
来源：http://gwk.feifeiyinyue.top

[R12] for 遍历文件
来源：http://axu.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://vof.ivvv.top

[R13] for 计数循环
来源：http://qvp.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://pbx.jyoumei.cn

[R14] C 风格 for
来源：http://jip.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qyy.meibo888.top

[R15] while 逐行读文件
来源：http://lru.zhongyouzk.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pog.316326.xyz

[R16] until 等待条件
来源：http://jqk.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cvo.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://usg.birdmap.top

arr=(a b c); echo "${arr[0]}"
来源：http://mpp.hysaishi.cn

[R18] 遍历数组
来源：http://hex.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uez.xinyue.icu

[R19] 数组长度
来源：http://hav.bbcook.cn

echo "${#arr[@]}"
来源：http://uql.xuanzx.com

[R20] 关联数组（字典）
来源：http://zov.cucudq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hnw.c1oappe.top

[R21] 字符串长度
来源：http://ciw.zhengqikj.top

echo "${#s}"
来源：http://xqm.gaohongyu789.top

[R22] 截取子串
来源：http://cpd.shzxlz.cn

echo "${s:0:5}"
来源：http://uut.tanke756.top

[R23] 字符串替换
来源：http://alg.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dxm.andypj.xyz

[R24] 大小写转换
来源：http://iym.yvedp.cn

echo "${s^^}"; echo "${s,,}"
来源：http://raa.fehbvm.com

[R25] 去后缀 / 去前缀
来源：http://fyp.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://dnm.sweek.top

[R26] 命令替换
来源：http://fdy.yonumen.top

now=$(date +%F); echo "$now"
来源：http://oua.pycfn.com

[R27] 算术展开
来源：http://oir.xziqi.cn

echo $((1 + 2 * 3))
来源：http://jzl.gogol.net.cn

[R28] 浮点运算
来源：http://str.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://zed.ybcxt.top

[R29] 定义函数
来源：http://cun.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jzh.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://kvh.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://xez.snrcjt.cn

[R31] 局部变量
来源：http://sli.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://gdd.vehdjk.com

[R32] 参数个数校验
来源：http://pkf.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hqu.smart0.xyz

[R33] 捕获错误并提示行号
来源：http://hwx.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qgh.zhoulong.xyz

[R34] 退出时清理
来源：http://tei.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://iuc.aibaodan.cn

[R35] 后台执行并等待
来源：http://ckt.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://idk.jlsjyb.cn

[R36] 并发执行多个任务
来源：http://tas.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://btf.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://udu.dianchejie.cn

files=$(ls -1)
来源：http://pgl.chenlongwang.top

[R38] 管道串联
来源：http://wau.meibo888.top

cat a.txt | grep -i error | wc -l
来源：http://jqr.cashguo.top

[R39] 重定向标准输出与错误
来源：http://vnm.iojbl.cn

cmd > out.log 2>&1
来源：http://fja.ivvv.top

[R40] 追加写日志
来源：http://iss.meibo888.top

echo "log" >> out.log
来源：http://jui.yanxiufei.cn

[R41] 丢弃输出
来源：http://rwn.zdqjudy.top

cmd >/dev/null 2>&1
来源：http://ypk.hfpthk.cn

[R42] 输入重定向
来源：http://ejt.yj20258888.top

wc -l < a.txt
来源：http://ust.sxryk.cn

[R43] 按名字查找文件
来源：http://rbk.sufxvd.cn

find . -name "*.log" -type f
来源：http://ceq.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://sir.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://due.wangdashe.top

[R45] 批量删除
来源：http://gqk.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://ayw.tianlin.xyz

[R46] 递归替换文件内容
来源：http://gpj.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://muh.hongshengwenyu.top

[R47] sed 单行替换
来源：http://fno.daxiang520.top

sed -i 's/foo/bar/g' a.txt
来源：http://ybx.gogol.net.cn

[R48] awk 取指定列
来源：http://jlq.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://kfy.jqgufenzy.top

[R49] awk 带条件
来源：http://qxx.c1oappe.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://azu.zdqjudy.top

[R50] awk 求和
来源：http://gta.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://ovz.yfazqb.com

[R51] 排序去重取前几
来源：http://emb.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://blt.xuetiantiany.cn

[R52] 统计行数
来源：http://wxn.zhiwuduotai.top

wc -l a.txt
来源：http://fdl.zhoulong.xyz

[R53] 查看文件头与实时尾
来源：http://lcl.nanxinkj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jjp.vqdsnc.cn

[R54] 比较两个文件
来源：http://tvt.gotoacloud.top

diff a.txt b.txt
来源：http://whu.gaohongyu789.top

[R55] 压缩与解压
来源：http://mlf.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xia.zhengqikj.top

[R56] 远程拷贝
来源：http://tff.zhongyouzk.top

scp file user@host:/path/
来源：http://vcz.hammf.cn

[R57] 远程执行命令
来源：http://qde.andypj.xyz

ssh user@host 'uptime'
来源：http://fes.gaohongyu789.top

[R58] 下载文件
来源：http://med.guannengcc.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vlq.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://kvo.guowangkeji.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zso.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://qfe.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xib.yonumen.top

[R61] 磁盘占用
来源：http://lwl.hnqzz.top

df -h;  du -sh *
来源：http://kpo.uphjek.com

[R62] 找最占空间的文件
来源：http://vre.tanke756.top

du -ah . | sort -rh | head -10
来源：http://zxx.sweek.top

[R63] 内存与进程
来源：http://hsj.shanyushiyangtech.top

free -h;  ps aux | grep nginx
来源：http://ssz.xylfe.cn

[R64] 结束进程
来源：http://zwn.316326.xyz

kill -9 $(pgrep -f app.py)
来源：http://xej.zhiwuduotai.top

[R65] 查看端口占用
来源：http://tpp.ywan-chungtsiang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vpb.cqqwz.cn

[R66] 定时任务
来源：http://woa.hysaishi.cn

crontab -e;  crontab -l
来源：http://oph.xylfe.cn

[R67] 生成随机十六进制串
来源：http://pgn.cqqwz.cn

openssl rand -hex 16
来源：http://tnr.smart0.xyz

[R68] 计算文件校验值
来源：http://ejw.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://nur.bjfxy.top

[R69] 生成随机密码
来源：http://kue.yangfankeji.com


<!-- 参考信息 -->