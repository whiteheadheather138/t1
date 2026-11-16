代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://poz.fktsv.cn

[Q24] 去重
来源：http://sud.quarkkingdee.top

SELECT DISTINCT city FROM users;
来源：http://qei.sysykeji.top

[Q25] 只取前 N 条
来源：http://ttf.nwbrower.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://day.epnwcf.com

[Q26] 计数
来源：http://msn.sjlbkw.cn

SELECT COUNT(*) FROM users;
来源：http://jxp.jqgfzy.top

[Q27] 条件计数
来源：http://uol.aizwys.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://hic.ydzc1.top

[Q28] 求和与平均
来源：http://dos.jianghu66.top

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://hfc.xylfe.cn

[Q29] 最大最小值
来源：http://sre.yfazqb.com

SELECT MAX(age), MIN(age) FROM users;
来源：http://joi.tanke756.top

[Q30] 分组统计
来源：http://mfu.yfazqb.com

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://djq.zdqjudy.top

[Q31] 分组后过滤
来源：http://qqf.52xcode.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://lel.jqgfzy.top

[Q32] 分组拼接字符串
来源：http://nph.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://rhz.fanxiaobao.xyz

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://rpi.shuidangran.top

[Q33] 多列分组
来源：http://htr.chenjidiqi.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://opk.daxiang520.top

[Q34] 每组取第一条
来源：http://ctq.sxryk.cn

SELECT * FROM (
来源：http://nsc.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://vdz.cdnleiting.top

) t WHERE rn = 1;
来源：http://uub.jlsjyb.cn

[Q35] 内连接
来源：http://toz.xylfe.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://osx.tanke756.top

[Q36] 左连接
来源：http://prk.snrcjt.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://bcg.fanxiaobao.xyz

[Q37] 右连接
来源：http://mpm.sufxvd.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://eky.yonumen.top

[Q38] 全外连接（PostgreSQL）
来源：http://bhz.ydzc1.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dke.smart0.xyz

[Q39] 自连接（查上下级）
来源：http://cps.fanxiaobao.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://jdl.xuanzx.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://umv.daxiang520.top

[Q40] 交叉连接（笛卡尔积）
来源：http://pwg.cheryme.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://nql.fanxiaobao.xyz

[Q41] 多表连接
来源：http://szp.hongshengwenyu.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://pvz.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://pjn.zdbjq.cn

JOIN products p ON p.id = o.product_id;
来源：http://ezm.hnxiangtu.top

[Q42] 连接条件附加过滤
来源：http://pbf.ybcxt.top

SELECT u.name, o.amount FROM users u
来源：http://mrm.jinqigfzy.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fgf.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://yxr.jiagoushi.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ndc.guannengcc.top

[Q44] IN 子查询
来源：http://pvj.316326.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://kan.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://niw.hfpthk.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://atb.jinghuilouyu.cn

[Q46] NOT EXISTS 判断不存在
来源：http://vcj.ybcxt.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rqm.yuanzhike.top

[Q47] 与平均值比较
来源：http://cap.pycfn.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pkn.yj20258.top

[Q48] CTE 公用表表达式
来源：http://vvs.yuxming.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ikj.wangdashe.top

SELECT * FROM t WHERE c > 5;
来源：http://izp.shuidangran.top

[Q49] 更新单行
来源：http://zkp.yfazqb.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vth.hammf.cn

[Q50] 批量更新
来源：http://wjn.kuanghao11.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://yeo.9152youxi.cn

[Q51] 用子查询更新
来源：http://vlw.daria6918.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hwb.yfazqb.com

[Q52] 删除指定行
来源：http://upf.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://mkh.quarkkingdee.top

[Q53] 按条件删除
来源：http://xmi.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wxn.bjfxy.top

[Q54] 清空表
来源：http://rnr.zhongyouzk.top

TRUNCATE TABLE logs;
来源：http://jfx.zdbjq.cn

[Q55] 排名（并列占位）
来源：http://fay.haohaochexian.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://kfe.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://mmh.cdnleiting.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fve.aizwys.cn

[Q57] 行号
来源：http://upa.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wae.ydjk.org.cn

[Q58] 累计求和
来源：http://pfc.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xku.aibaodan.cn

[Q59] 分组内累计
来源：http://edf.cheryme.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jif.smart0.xyz

[Q60] 取上一行 / 下一行
来源：http://wic.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://rqt.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fux.c1oappe.top

[Q61] 移动平均
来源：http://fdc.feifeiyinyue.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ynr.jlsjyb.cn

[Q62] 分组占比
来源：http://xtd.xuetiantiany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jmu.hnqzz.top

[Q63] 开启事务
来源：http://sze.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pbc.uphjek.com

[Q64] 提交事务
来源：http://gdt.hongshengwenyu.top

COMMIT;
来源：http://kzb.jinghuilouyu.cn

[Q65] 回滚事务
来源：http://qtf.svipenyu.cn

ROLLBACK;
来源：http://xaa.yonumen.top

[Q66] 行锁查询
来源：http://izi.yj202588.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ihw.jinghuilouyu.cn

[Q67] 设置隔离级别
来源：http://pyh.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://szi.ppjwa.cn

[Q68] 保存点
来源：http://fjj.haohaochexian.top

SAVEPOINT sp1;
来源：http://vjr.zdqjudy.top

ROLLBACK TO sp1;
来源：http://mtk.meibo888.top

[Q69] 查看执行计划
来源：http://xut.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vtk.snrcjt.cn

[Q70] 更新统计信息
来源：http://dts.iojbl.cn

ANALYZE TABLE users;
来源：http://qoa.redwolf501.top

[Q71] 查看建表语句
来源：http://wms.zdqjudy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uyj.fktsv.cn

[Q72] 查看索引
来源：http://pjp.pengpengdd.cyou

SHOW INDEX FROM users;
来源：http://wbb.hesvh.cn

[Q73] 查看表状态
来源：http://bsk.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fuv.andypj.xyz

[Q74] 强制使用索引
来源：http://tmx.ctjpmb.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zwu.pycfn.com

[Q75] 日期格式化
来源：http://exi.zhongyouzk.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://syl.sweek.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jrm.sysykeji.top

[Q76] 按天统计
来源：http://nrd.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dcv.gotoacloud.top

[Q77] 时间加减
来源：http://tcs.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zck.nwbrower.top

[Q78] 当前时间
来源：http://gls.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://opx.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://sdk.hywenlv.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sum.hongshengwenyu.top

[Q80] 字符串截取
来源：http://yex.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://akn.tian-w.cn

[Q81] 字符串替换
来源：http://kaz.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nmj.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://txx.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kjq.yj202588.top

[Q83] 大小写转换
来源：http://omk.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://woh.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://fwj.zycfv.cn

SELECT TRIM(name) FROM users;
来源：http://dep.xziqi.cn

[Q85] 数值取整
来源：http://gnz.hongshengwenyu.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yag.fzhhl.top

[Q86] 读取 JSON 字段
来源：http://tyj.jinqigufen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pdg.meibo888.top

[Q87] JSON 字段做条件
来源：http://giy.hywenlv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrw.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://xwt.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rcy.shanyushiyangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bjp.tian-w.cn

[Q89] 判断表是否存在
来源：http://nrr.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qpu.cashguo.top

[Q90] 生成序号列
来源：http://dfk.shuidangran.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qxp.yj20258.top

================================================================================
来源：http://fsb.snrcjt.cn

R. Bash 专题
来源：http://pjy.0kj1m.cn

================================================================================
来源：http://jfu.hammf.cn

[R01] shebang 与严格模式
来源：http://bba.cashguo.top

#!/usr/bin/env bash
来源：http://qij.52xcode.cn

set -euo pipefail
来源：http://znh.cucudq.cn

[R02] 变量赋值与使用
来源：http://fbl.jiagoushi.top

name="Tom"; echo "$name"
来源：http://ywz.guowangkeji.top

[R03] 只读变量
来源：http://ttl.zhongyouzk.top

readonly PI=3.14
来源：http://kzv.zhaomingkeji.xyz

[R04] 位置参数
来源：http://fyi.shuidangran.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hjl.fzhhl.top

[R05] 参数默认值
来源：http://wjd.xuetiantiany.cn

name="${1:-default}"
来源：http://jdd.meibo888.top

[R06] 判断命令是否存在
来源：http://opi.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wab.jianghu66.top

[R07] if 判断文件
来源：http://xaj.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yan.hnqzz.top

[R08] 数值比较
来源：http://mrv.jqgfzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bwv.fengsongda.top

[R09] 字符串比较
来源：http://yvr.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mqt.guowangkeji.top

[R10] 正则匹配
来源：http://fag.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://oqg.birdmap.top

[R11] case 多分支
来源：http://irg.yanxiufei.cn

case "$1" in
来源：http://ezs.jinghuilouyu.cn

start) echo "启动" ;;
来源：http://uqy.yangfankeji.com

stop)  echo "停止" ;;
来源：http://vio.havefunace.top

*)     echo "未知命令" ;;
来源：http://jnu.jyoumei.cn

esac
来源：http://cst.xuetiantiany.cn

[R12] for 遍历文件
来源：http://clk.zhoulong.xyz

for f in *.txt; do echo "$f"; done
来源：http://dee.daria6918.cn

[R13] for 计数循环
来源：http://khe.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://aqj.bjfxy.top

[R14] C 风格 for
来源：http://rah.bjfxy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://htb.dianchejie.cn

[R15] while 逐行读文件
来源：http://jqd.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ska.chenjidiqi.icu

[R16] until 等待条件
来源：http://wjh.andypj.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tsj.c1oappe.top

[R17] 数组定义与取值
来源：http://kei.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://nww.jinghuilouyu.cn

[R18] 遍历数组
来源：http://jyj.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nem.snrcjt.cn

[R19] 数组长度
来源：http://jwx.andypj.xyz

echo "${#arr[@]}"
来源：http://hts.cqqwz.cn

[R20] 关联数组（字典）
来源：http://sux.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jmt.gzhubu.top

[R21] 字符串长度
来源：http://qdn.bbcook.cn

echo "${#s}"
来源：http://cib.pycfn.com

[R22] 截取子串
来源：http://vvv.jiagoushi.top

echo "${s:0:5}"
来源：http://thc.gzhubu.top

[R23] 字符串替换
来源：http://wdq.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zjd.haohaochexian.top

[R24] 大小写转换
来源：http://hrf.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://lve.zdqjudy.top

[R25] 去后缀 / 去前缀
来源：http://hjv.sxryk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://uye.xylfe.cn

[R26] 命令替换
来源：http://kkk.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://alt.andypj.xyz

[R27] 算术展开
来源：http://fso.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://rnl.yvedp.cn

[R28] 浮点运算
来源：http://klq.yuxming.cn

echo "scale=2; 10/3" | bc
来源：http://nmf.snrcjt.cn

[R29] 定义函数
来源：http://azm.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fak.jlsjyb.cn

[R30] 函数返回状态码
来源：http://epb.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://dcd.xinyue.icu

[R31] 局部变量
来源：http://hlg.ivvv.top

f() { local x=1; echo "$x"; }
来源：http://ubv.guannengcc.top

[R32] 参数个数校验
来源：http://gri.sufxvd.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jbe.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://vjy.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pag.birdmap.top

[R34] 退出时清理
来源：http://atw.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ved.zhixingplan.top

[R35] 后台执行并等待
来源：http://eox.epnwcf.com

sleep 5 & pid=$!; wait "$pid"
来源：http://jxg.dashuyun.cn

[R36] 并发执行多个任务
来源：http://oeb.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jxv.gogol.net.cn

[R37] 把输出赋给变量
来源：http://vpk.xziqi.cn

files=$(ls -1)
来源：http://mzl.zhongyouzk.top

[R38] 管道串联
来源：http://trr.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://unt.0kj1m.cn

[R39] 重定向标准输出与错误
来源：http://wng.zhengqikj.top

cmd > out.log 2>&1
来源：http://wnr.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://xcs.xuetiantiany.cn

echo "log" >> out.log
来源：http://tka.sysykeji.top

[R41] 丢弃输出
来源：http://gcv.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://ely.fanxiaobao.xyz

[R42] 输入重定向
来源：http://alu.redwolf501.top

wc -l < a.txt
来源：http://dqu.xinyue.icu

[R43] 按名字查找文件
来源：http://voi.ehwqpu.com

find . -name "*.log" -type f
来源：http://ddd.yanxiufei.cn

[R44] 按修改时间查找
来源：http://nvp.0kj1m.cn

find . -mtime -7 -type f
来源：http://yhv.sjlbkw.cn

[R45] 批量删除
来源：http://gpa.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://job.zdqjudy.top

[R46] 递归替换文件内容
来源：http://tod.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ggp.xuetiantiany.cn

[R47] sed 单行替换
来源：http://vnw.xziqi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://glp.svipenyu.cn

[R48] awk 取指定列
来源：http://hmp.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://svx.andypj.xyz

[R49] awk 带条件
来源：http://dbh.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kni.wangshuangyany.cn

[R50] awk 求和
来源：http://yrz.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fyh.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://zlt.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dmc.c1oappe.top

[R52] 统计行数
来源：http://fuh.sxryk.cn

wc -l a.txt
来源：http://yvv.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://tbc.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://whg.sysykeji.top

[R54] 比较两个文件
来源：http://bey.pycfn.com

diff a.txt b.txt
来源：http://egm.sxryk.cn

[R55] 压缩与解压
来源：http://vqz.zhijiandao.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eyu.yueranfly.top

[R56] 远程拷贝
来源：http://vvs.fanxiaobao.xyz

scp file user@host:/path/
来源：http://yml.aizwys.cn

[R57] 远程执行命令
来源：http://dzz.haohaochexian.top

ssh user@host 'uptime'
来源：http://fcs.birdmap.top

[R58] 下载文件
来源：http://uwy.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tdc.gotoacloud.top

[R59] 发 POST JSON
来源：http://azo.hywenlv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sbo.iojbl.cn

[R60] 只看 HTTP 状态码
来源：http://nhu.zdqjudy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nmy.chenlongwang.top

[R61] 磁盘占用
来源：http://mya.tianlin.xyz

df -h;  du -sh *
来源：http://umm.pengpengdd.cyou

[R62] 找最占空间的文件
来源：http://itt.smart0.xyz

du -ah . | sort -rh | head -10
来源：http://kiu.hnqzz.top

[R63] 内存与进程
来源：http://hif.shangyingyoupin.top

free -h;  ps aux | grep nginx
来源：http://hwa.jqgfzy.top

[R64] 结束进程
来源：http://cmx.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://qrs.shanyushiyangtech.top

[R65] 查看端口占用
来源：http://bha.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://adn.kuanghao11.cn

[R66] 定时任务
来源：http://cqg.chenlongwang.top

crontab -e;  crontab -l
来源：http://dvf.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://dtu.ydzc1.top

openssl rand -hex 16
来源：http://ccl.ctjpmb.com

[R68] 计算文件校验值
来源：http://iuj.ctjpmb.com

sha256sum a.txt;  md5sum a.txt
来源：http://lzk.sjlbkw.cn

[R69] 生成随机密码
来源：http://izs.snrcjt.cn

head -c 16 /dev/urandom | base64
来源：http://tng.gogol.net.cn

[R70] 时间戳与互转
来源：http://pih.yj202588.top

date +%s;  date -d @1700000000
来源：http://axn.zhengqikj.top

[R71] 日期格式化
来源：http://jmw.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ltz.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://gmc.nwbrower.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lom.smart0.xyz

[R73] 分割大日志
来源：http://vpw.ctjpmb.com


<!-- 参考信息 -->