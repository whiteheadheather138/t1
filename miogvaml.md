代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://aeb.zhixingplan.top

[Q26] 计数
来源：http://bca.zhaomingkeji.xyz

SELECT COUNT(*) FROM users;
来源：http://wnu.yj20258888.top

[Q27] 条件计数
来源：http://jtq.zhaomingkeji.xyz

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://ekh.tianlin.xyz

[Q28] 求和与平均
来源：http://bht.ctjpmb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://nfg.feifeiyinyue.top

[Q29] 最大最小值
来源：http://dao.pengpengdd.cyou

SELECT MAX(age), MIN(age) FROM users;
来源：http://hxm.cashguo.top

[Q30] 分组统计
来源：http://bbz.epnwcf.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ndg.9152youxi.cn

[Q31] 分组后过滤
来源：http://zcc.ppjwa.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lxo.nanxinkj.top

[Q32] 分组拼接字符串
来源：http://ewb.aibaodan.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://sjw.ehwqpu.com

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://uza.yanxiufei.cn

[Q33] 多列分组
来源：http://wkb.xylfe.cn

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ojq.zhaomingkeji.xyz

[Q34] 每组取第一条
来源：http://uon.jqgfzy.top

SELECT * FROM (
来源：http://jcu.yuxming.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ipr.gaohongyu789.top

) t WHERE rn = 1;
来源：http://iul.chenjidiqi.icu

[Q35] 内连接
来源：http://sfq.yueranfly.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://taf.cashguo.top

[Q36] 左连接
来源：http://ryb.shangyingyoupin.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://sev.0kj1m.cn

[Q37] 右连接
来源：http://lwx.yfazqb.com

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eoq.yueranfly.top

[Q38] 全外连接（PostgreSQL）
来源：http://dnc.xingfuxueyuan.xyz

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qhm.0kj1m.cn

[Q39] 自连接（查上下级）
来源：http://zqg.gaohongyu789.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://isy.snrcjt.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tnd.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://jmy.yfazqb.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ikp.hammf.cn

[Q41] 多表连接
来源：http://qbz.xuetiantiany.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vva.fanxiaobao.xyz

JOIN users u ON u.id = o.user_id
来源：http://jzl.fehbvm.com

JOIN products p ON p.id = o.product_id;
来源：http://nlx.mhx1999.top

[Q42] 连接条件附加过滤
来源：http://frs.tanke756.top

SELECT u.name, o.amount FROM users u
来源：http://dlu.yangfankeji.com

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://qku.aibaodan.cn

[Q43] 标量子查询
来源：http://vls.52xcode.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jnc.havefunace.top

[Q44] IN 子查询
来源：http://ycg.xziqi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hiq.cdnleiting.top

[Q45] EXISTS 判断存在
来源：http://zug.sxryk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lco.9152youxi.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yfg.birdmap.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nyl.zycfv.cn

[Q47] 与平均值比较
来源：http://ica.ydzc1.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://uci.shanyushiyangtech.top

[Q48] CTE 公用表表达式
来源：http://dvz.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nas.hfpthk.cn

SELECT * FROM t WHERE c > 5;
来源：http://xlo.yj20258.top

[Q49] 更新单行
来源：http://pop.svipenyu.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pek.aibaodan.cn

[Q50] 批量更新
来源：http://cgp.yfazqb.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kho.wangshuangyany.cn

[Q51] 用子查询更新
来源：http://lfv.chenlongwang.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ftb.redwolf501.top

[Q52] 删除指定行
来源：http://dmt.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://iiz.nanxinkj.top

[Q53] 按条件删除
来源：http://csm.ehwqpu.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://obz.jinqigfzy.top

[Q54] 清空表
来源：http://kou.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://xfb.hywenlv.cn

[Q55] 排名（并列占位）
来源：http://rgq.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qwz.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://uao.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oex.jiagoushi.top

[Q57] 行号
来源：http://qkw.dashuyun.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://egh.9152youxi.cn

[Q58] 累计求和
来源：http://dek.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lxe.vehdjk.com

[Q59] 分组内累计
来源：http://tyo.vehdjk.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kxc.zhoulong.xyz

[Q60] 取上一行 / 下一行
来源：http://rvr.cdnleiting.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://whx.wangshuangyany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cjn.zhongyouzk.top

[Q61] 移动平均
来源：http://sdz.ywan-chungtsiang.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://qyd.fanxiaobao.xyz

[Q62] 分组占比
来源：http://gzr.ivvv.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vwv.fehbvm.com

[Q63] 开启事务
来源：http://zop.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://jac.birdmap.top

[Q64] 提交事务
来源：http://wdw.chenjidiqi.icu

COMMIT;
来源：http://kok.sweek.top

[Q65] 回滚事务
来源：http://vqd.meibo888.top

ROLLBACK;
来源：http://ged.hnqzz.top

[Q66] 行锁查询
来源：http://laa.dashuyun.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xlw.yangfankeji.com

[Q67] 设置隔离级别
来源：http://fxy.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hof.zhongyouzk.top

[Q68] 保存点
来源：http://kkp.jinqigfzy.top

SAVEPOINT sp1;
来源：http://pot.shuidangran.top

ROLLBACK TO sp1;
来源：http://jud.zdqjudy.top

[Q69] 查看执行计划
来源：http://yvc.dashuyun.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uri.yongpay.top

[Q70] 更新统计信息
来源：http://pen.zhiwuduotai.top

ANALYZE TABLE users;
来源：http://ajs.aizwys.cn

[Q71] 查看建表语句
来源：http://udi.haohaochexian.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pzs.aizwys.cn

[Q72] 查看索引
来源：http://udq.cashguo.top

SHOW INDEX FROM users;
来源：http://bqa.havefunace.top

[Q73] 查看表状态
来源：http://ftj.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://vyd.yongpay.top

[Q74] 强制使用索引
来源：http://lhi.cqqwz.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bvg.tanke756.top

[Q75] 日期格式化
来源：http://ouz.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gnf.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ptm.yonumen.top

[Q76] 按天统计
来源：http://zvk.ydjk.org.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nld.tian-w.cn

[Q77] 时间加减
来源：http://zmc.hywenlv.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kmn.ivvv.top

[Q78] 当前时间
来源：http://pgl.yonumen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vcs.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://abq.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rmp.hcnkem.com

[Q80] 字符串截取
来源：http://ijc.zycfv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bor.iojbl.cn

[Q81] 字符串替换
来源：http://pfm.zhaomingkeji.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wcj.cheryme.top

[Q82] 字符长度与字节长度
来源：http://pig.sufxvd.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pce.mhx1999.top

[Q83] 大小写转换
来源：http://lwu.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mtb.nanxinkj.top

[Q84] 去除首尾空格
来源：http://jcm.yvedp.cn

SELECT TRIM(name) FROM users;
来源：http://gka.jqgfzy.top

[Q85] 数值取整
来源：http://exp.yj20258888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://opt.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://cob.xinyue.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zqg.xuetiantiany.cn

[Q87] JSON 字段做条件
来源：http://alh.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://azc.zhaomingkeji.xyz

[Q88] 行转列（条件聚合）
来源：http://kis.zdqjudy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vyv.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://taa.vehdjk.com

[Q89] 判断表是否存在
来源：http://imw.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pca.cdnleiting.top

[Q90] 生成序号列
来源：http://ucj.cdnleiting.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nnp.chenzaomai.com

================================================================================
来源：http://rbu.nanxinkj.top

R. Bash 专题
来源：http://bzq.quarkkingdee.top

================================================================================
来源：http://byz.ctjpmb.com

[R01] shebang 与严格模式
来源：http://rju.bbcook.cn

#!/usr/bin/env bash
来源：http://izm.havefunace.top

set -euo pipefail
来源：http://mtm.zdbjq.cn

[R02] 变量赋值与使用
来源：http://egn.fzhhl.top

name="Tom"; echo "$name"
来源：http://ool.xingfuxueyuan.xyz

[R03] 只读变量
来源：http://sdp.xinyue.icu

readonly PI=3.14
来源：http://vyo.tarul.cn

[R04] 位置参数
来源：http://wcy.xuanzx.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bbz.birdmap.top

[R05] 参数默认值
来源：http://ffs.fzhhl.top

name="${1:-default}"
来源：http://lui.aizwys.cn

[R06] 判断命令是否存在
来源：http://isw.snrcjt.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nfb.cucudq.cn

[R07] if 判断文件
来源：http://hwk.epnwcf.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bsu.dianchejie.cn

[R08] 数值比较
来源：http://was.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://mis.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://jyw.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lxv.jlsjyb.cn

[R10] 正则匹配
来源：http://ihm.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rhn.zhoulong.xyz

[R11] case 多分支
来源：http://esv.wangdashe.top

case "$1" in
来源：http://uwp.c1oappe.top

start) echo "启动" ;;
来源：http://ezj.yuxming.cn

stop)  echo "停止" ;;
来源：http://jjd.svipenyu.cn

*)     echo "未知命令" ;;
来源：http://lac.cqqwz.cn

esac
来源：http://nvx.dashuyun.cn

[R12] for 遍历文件
来源：http://ouy.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://kmb.tian-w.cn

[R13] for 计数循环
来源：http://gfi.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://pko.yj20258.top

[R14] C 风格 for
来源：http://vxr.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wvl.chenlongwang.top

[R15] while 逐行读文件
来源：http://vyz.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nmo.redwolf501.top

[R16] until 等待条件
来源：http://uwi.nanxuanxn.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wnj.uphjek.com

[R17] 数组定义与取值
来源：http://gfj.hnqzz.top

arr=(a b c); echo "${arr[0]}"
来源：http://cfq.cashguo.top

[R18] 遍历数组
来源：http://lhq.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bkr.havefunace.top

[R19] 数组长度
来源：http://vgb.daria6918.cn

echo "${#arr[@]}"
来源：http://jzj.9152youxi.cn

[R20] 关联数组（字典）
来源：http://aiw.gaohongyu789.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yha.hysaishi.cn

[R21] 字符串长度
来源：http://nih.nwbrower.top

echo "${#s}"
来源：http://vsz.fengsongda.top

[R22] 截取子串
来源：http://bfk.gzhubu.top

echo "${s:0:5}"
来源：http://eak.fanxiaobao.xyz

[R23] 字符串替换
来源：http://phd.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wkj.cheryme.top

[R24] 大小写转换
来源：http://uhg.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://sgq.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://hqt.jinqigfzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vcj.nanxinkj.top

[R26] 命令替换
来源：http://qek.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://omw.aizwys.cn

[R27] 算术展开
来源：http://fiz.nanxinkj.top

echo $((1 + 2 * 3))
来源：http://vlt.ivvv.top

[R28] 浮点运算
来源：http://pwi.yangfankeji.com

echo "scale=2; 10/3" | bc
来源：http://yml.daria6918.cn

[R29] 定义函数
来源：http://zok.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yic.ctjpmb.com

[R30] 函数返回状态码
来源：http://isx.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://vdt.svipenyu.cn

[R31] 局部变量
来源：http://lfv.jinghuilouyu.cn

f() { local x=1; echo "$x"; }
来源：http://yrv.sweek.top

[R32] 参数个数校验
来源：http://mhi.ivvv.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vcj.snrcjt.cn

[R33] 捕获错误并提示行号
来源：http://fag.nwbrower.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qkv.yj202588.top

[R34] 退出时清理
来源：http://pfo.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://rbb.zhoulong.xyz

[R35] 后台执行并等待
来源：http://vze.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wpb.hfpthk.cn

[R36] 并发执行多个任务
来源：http://yxa.shanyushiyangtech.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vyc.52xcode.cn

[R37] 把输出赋给变量
来源：http://hlz.shuidangran.top

files=$(ls -1)
来源：http://hkx.fehbvm.com

[R38] 管道串联
来源：http://nwk.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://saq.nwbrower.top

[R39] 重定向标准输出与错误
来源：http://jno.snrcjt.cn

cmd > out.log 2>&1
来源：http://xkj.gogol.net.cn

[R40] 追加写日志
来源：http://roo.yonumen.top

echo "log" >> out.log
来源：http://mep.gogol.net.cn

[R41] 丢弃输出
来源：http://uty.jinyuanbaomall.cn

cmd >/dev/null 2>&1
来源：http://jiw.shzxlz.cn

[R42] 输入重定向
来源：http://iyl.jyoumei.cn

wc -l < a.txt
来源：http://efo.daria6918.cn

[R43] 按名字查找文件
来源：http://ljs.hnxiangtu.top

find . -name "*.log" -type f
来源：http://shh.sweek.top

[R44] 按修改时间查找
来源：http://yin.cheryme.top

find . -mtime -7 -type f
来源：http://wjt.snrcjt.cn

[R45] 批量删除
来源：http://ovs.wangdashe.top

find . -name "*.tmp" -delete
来源：http://bcw.nanxinkj.top

[R46] 递归替换文件内容
来源：http://gkf.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yjl.wangshuangyany.cn

[R47] sed 单行替换
来源：http://qjl.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://kgv.ydjk.org.cn

[R48] awk 取指定列
来源：http://ard.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://uzh.mhx1999.top

[R49] awk 带条件
来源：http://zoz.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://amt.jinqigufen.top

[R50] awk 求和
来源：http://aaf.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://dpu.yvedp.cn

[R51] 排序去重取前几
来源：http://elc.fehbvm.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xhu.aizwys.cn

[R52] 统计行数
来源：http://lku.52xcode.cn

wc -l a.txt
来源：http://ksu.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://wzg.jinqigufen.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ltl.yj20258888.top

[R54] 比较两个文件
来源：http://rcq.sxryk.cn

diff a.txt b.txt
来源：http://ace.aibaodan.cn

[R55] 压缩与解压
来源：http://glu.daxiang520.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xid.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://enx.fzhhl.top

scp file user@host:/path/
来源：http://tnk.yj202588.top

[R57] 远程执行命令
来源：http://zid.iojbl.cn

ssh user@host 'uptime'
来源：http://zwo.xuanzx.com

[R58] 下载文件
来源：http://yml.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ekf.hesvh.cn

[R59] 发 POST JSON
来源：http://abp.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://quo.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://pzz.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fab.yj20258.top

[R61] 磁盘占用
来源：http://uxe.dianchejie.cn

df -h;  du -sh *
来源：http://jjt.jiagoushi.top

[R62] 找最占空间的文件
来源：http://rpn.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://mco.aibaodan.cn

[R63] 内存与进程
来源：http://xrq.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://ifd.sxryk.cn

[R64] 结束进程
来源：http://nmz.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://wtp.andypj.xyz

[R65] 查看端口占用
来源：http://yah.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ybl.daria6918.cn

[R66] 定时任务
来源：http://npm.zhijiandao.cn

crontab -e;  crontab -l
来源：http://ovu.jqgufenzy.top

[R67] 生成随机十六进制串
来源：http://aco.jianghu66.top

openssl rand -hex 16
来源：http://ckg.pycfn.com

[R68] 计算文件校验值
来源：http://imx.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kag.xylfe.cn

[R69] 生成随机密码
来源：http://ohy.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://voe.xziqi.cn

[R70] 时间戳与互转
来源：http://uqz.hesvh.cn

date +%s;  date -d @1700000000
来源：http://aml.yuxming.cn

[R71] 日期格式化
来源：http://lly.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tfx.shzxlz.cn

[R72] 等待端口就绪
来源：http://kdu.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://cfq.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://dsz.hongshengwenyu.top

split -l 1000 big.log part_
来源：http://iyi.xuanzx.com

[R74] 批量重命名
来源：http://bsh.fanxiaobao.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rqt.redwolf501.top

[R75] 导出环境变量
来源：http://osf.yangfankeji.com


<!-- 参考信息 -->