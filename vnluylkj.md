代发 wailian999

[Q33] 多列分组
来源：http://cuh.ctjpmb.com

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://idf.zdbjq.cn

[Q34] 每组取第一条
来源：http://ttv.feifeiyinyue.top

SELECT * FROM (
来源：http://cak.ybcxt.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://rll.fktsv.cn

) t WHERE rn = 1;
来源：http://ibf.hfpthk.cn

[Q35] 内连接
来源：http://lmg.hfpthk.cn

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://rap.52xcode.cn

[Q36] 左连接
来源：http://uph.zhijiandao.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://yfa.yuanzhike.top

[Q37] 右连接
来源：http://xgb.cashguo.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://auq.guannengcc.top

[Q38] 全外连接（PostgreSQL）
来源：http://gfd.daria6918.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dcl.fzhhl.top

[Q39] 自连接（查上下级）
来源：http://gko.9152youxi.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://nhg.redwolf501.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tgy.yj202588.top

[Q40] 交叉连接（笛卡尔积）
来源：http://qft.zdqjudy.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hgu.tian-w.cn

[Q41] 多表连接
来源：http://uge.yonumen.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://qkg.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://wnl.yuanzhike.top

JOIN products p ON p.id = o.product_id;
来源：http://xtn.hcnkem.com

[Q42] 连接条件附加过滤
来源：http://hsh.aibaodan.cn

SELECT u.name, o.amount FROM users u
来源：http://uqu.andypj.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jgc.9152youxi.cn

[Q43] 标量子查询
来源：http://qdh.c1oappe.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://fdc.zycfv.cn

[Q44] IN 子查询
来源：http://ytq.sysykeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://gin.hnqzz.top

[Q45] EXISTS 判断存在
来源：http://got.yuxming.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kip.cucudq.cn

[Q46] NOT EXISTS 判断不存在
来源：http://rie.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://orz.chenjidiqi.icu

[Q47] 与平均值比较
来源：http://ptp.cucudq.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://llq.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://mvn.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://esy.hywenlv.cn

SELECT * FROM t WHERE c > 5;
来源：http://gsi.yueranfly.top

[Q49] 更新单行
来源：http://qjs.fengsongda.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nun.shzxlz.cn

[Q50] 批量更新
来源：http://byt.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nek.zhengqikj.top

[Q51] 用子查询更新
来源：http://aoa.shangyingyoupin.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xlk.gogol.net.cn

[Q52] 删除指定行
来源：http://rzf.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://ljz.zdqjudy.top

[Q53] 按条件删除
来源：http://wix.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rma.jianghu66.top

[Q54] 清空表
来源：http://hdo.hammf.cn

TRUNCATE TABLE logs;
来源：http://ewg.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://qzu.tanke756.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://laz.jqgufenzy.top

[Q56] 密集排名（并列不占位）
来源：http://hnt.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://iry.shuidangran.top

[Q57] 行号
来源：http://oyb.52xcode.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://eza.shuidangran.top

[Q58] 累计求和
来源：http://vvs.chenlongwang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jdg.mhx1999.top

[Q59] 分组内累计
来源：http://upq.hfpthk.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qwk.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://jux.52xcode.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ehf.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://djd.xziqi.cn

[Q61] 移动平均
来源：http://afc.shzxlz.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://piu.ctjpmb.com

[Q62] 分组占比
来源：http://zba.hongshengwenyu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kew.gaohongyu789.top

[Q63] 开启事务
来源：http://cik.feifeiyinyue.top

START TRANSACTION;                -- 或 BEGIN
来源：http://skx.daria6918.cn

[Q64] 提交事务
来源：http://qmr.shanyushiyangkeji.top

COMMIT;
来源：http://myl.yongpay.top

[Q65] 回滚事务
来源：http://jsk.meibo888.top

ROLLBACK;
来源：http://vhc.jinqigufen.top

[Q66] 行锁查询
来源：http://opl.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mek.redwolf501.top

[Q67] 设置隔离级别
来源：http://xgp.hammf.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zhm.dashuyun.cn

[Q68] 保存点
来源：http://cyn.tian-w.cn

SAVEPOINT sp1;
来源：http://asp.gogol.net.cn

ROLLBACK TO sp1;
来源：http://zui.yueranfly.top

[Q69] 查看执行计划
来源：http://stf.yvedp.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fxl.shangyingyoupin.top

[Q70] 更新统计信息
来源：http://fse.chenlongwang.top

ANALYZE TABLE users;
来源：http://dhh.zhiwuduotai.top

[Q71] 查看建表语句
来源：http://vpt.c1oappe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ppa.yonumen.top

[Q72] 查看索引
来源：http://ipe.yj20258.top

SHOW INDEX FROM users;
来源：http://lgn.dashuyun.cn

[Q73] 查看表状态
来源：http://vwf.fanxiaobao.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://xpy.guannengcc.top

[Q74] 强制使用索引
来源：http://giu.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://aey.hnqzz.top

[Q75] 日期格式化
来源：http://vej.xingfuxueyuan.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vfk.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iwr.cucudq.cn

[Q76] 按天统计
来源：http://syv.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://uub.chenlongwang.top

[Q77] 时间加减
来源：http://zmy.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oio.sxryk.cn

[Q78] 当前时间
来源：http://who.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yju.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://zdq.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ylu.cashguo.top

[Q80] 字符串截取
来源：http://cbb.9152youxi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://vwg.quarkkingdee.top

[Q81] 字符串替换
来源：http://dvt.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oeb.sufxvd.cn

[Q82] 字符长度与字节长度
来源：http://yql.nwbrower.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ctm.yuxming.cn

[Q83] 大小写转换
来源：http://dcf.sjlbkw.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wcz.shanyushiyangkeji.top

[Q84] 去除首尾空格
来源：http://axu.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://gpp.fehbvm.com

[Q85] 数值取整
来源：http://aub.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://skw.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://qho.yongpay.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kml.nwbrower.top

[Q87] JSON 字段做条件
来源：http://rmk.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jkq.gaohongyu789.top

[Q88] 行转列（条件聚合）
来源：http://ord.yangfankeji.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mjs.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eec.jinqigufen.top

[Q89] 判断表是否存在
来源：http://hpa.jinyuanbaomall.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yqg.zycfv.cn

[Q90] 生成序号列
来源：http://crs.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://amg.wangshuangyany.cn

================================================================================
来源：http://swu.zycfv.cn

R. Bash 专题
来源：http://eal.sjlbkw.cn

================================================================================
来源：http://ipu.dianchejie.cn

[R01] shebang 与严格模式
来源：http://scl.cqqwz.cn

#!/usr/bin/env bash
来源：http://lvi.fanxiaobao.xyz

set -euo pipefail
来源：http://mnv.fzhhl.top

[R02] 变量赋值与使用
来源：http://lhd.yongpay.top

name="Tom"; echo "$name"
来源：http://vhg.bjfxy.top

[R03] 只读变量
来源：http://bxv.uphjek.com

readonly PI=3.14
来源：http://rjq.zdbjq.cn

[R04] 位置参数
来源：http://jaj.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sle.hfpthk.cn

[R05] 参数默认值
来源：http://wtz.ctjpmb.com

name="${1:-default}"
来源：http://qcd.mhx1999.top

[R06] 判断命令是否存在
来源：http://lyw.feifeiyinyue.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bsg.fengsongda.top

[R07] if 判断文件
来源：http://hzh.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lvc.jinghuilouyu.cn

[R08] 数值比较
来源：http://npb.gogol.net.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dqc.xziqi.cn

[R09] 字符串比较
来源：http://whq.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ymw.fanxiaobao.xyz

[R10] 正则匹配
来源：http://aot.zycfv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vbs.ehwqpu.com

[R11] case 多分支
来源：http://rho.tanke756.top

case "$1" in
来源：http://egb.cqqwz.cn

start) echo "启动" ;;
来源：http://zmj.birdmap.top

stop)  echo "停止" ;;
来源：http://tox.yj20258.top

*)     echo "未知命令" ;;
来源：http://kqq.smart0.xyz

esac
来源：http://hds.bjfxy.top

[R12] for 遍历文件
来源：http://vtc.jqgufenzy.top

for f in *.txt; do echo "$f"; done
来源：http://her.xylfe.cn

[R13] for 计数循环
来源：http://ail.zhaomingkeji.xyz

for i in {1..10}; do echo "$i"; done
来源：http://moh.shanyushiyangtech.top

[R14] C 风格 for
来源：http://att.jinghuilouyu.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://dvz.jyoumei.cn

[R15] while 逐行读文件
来源：http://lyc.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lgr.zhixingplan.top

[R16] until 等待条件
来源：http://sdi.0kj1m.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ban.zhongyouzk.top

[R17] 数组定义与取值
来源：http://oqk.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vby.guannengcc.top

[R18] 遍历数组
来源：http://lig.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mcg.mhx1999.top

[R19] 数组长度
来源：http://caa.sxryk.cn

echo "${#arr[@]}"
来源：http://qcm.hfpthk.cn

[R20] 关联数组（字典）
来源：http://zcr.vqdsnc.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gfp.hywenlv.cn

[R21] 字符串长度
来源：http://gpu.smart0.xyz

echo "${#s}"
来源：http://hlr.zhengqikj.top

[R22] 截取子串
来源：http://apt.zhiwuduotai.top

echo "${s:0:5}"
来源：http://xwx.gogol.net.cn

[R23] 字符串替换
来源：http://cst.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://tpw.gogol.net.cn

[R24] 大小写转换
来源：http://xbf.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gtv.chenzaomai.com

[R25] 去后缀 / 去前缀
来源：http://ypi.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://kxk.ppjwa.cn

[R26] 命令替换
来源：http://qyt.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://nec.zycfv.cn

[R27] 算术展开
来源：http://vhb.jianghu66.top

echo $((1 + 2 * 3))
来源：http://nga.meibo888.top

[R28] 浮点运算
来源：http://ibq.0kj1m.cn

echo "scale=2; 10/3" | bc
来源：http://rbi.gzhubu.top

[R29] 定义函数
来源：http://ann.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://abr.nanxuanxn.top

[R30] 函数返回状态码
来源：http://hfh.shanyushiyangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://jzh.guannengcc.top

[R31] 局部变量
来源：http://uxs.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://gty.316326.xyz

[R32] 参数个数校验
来源：http://dov.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jls.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://hsa.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ydz.zhongyouzk.top

[R34] 退出时清理
来源：http://wki.vqdsnc.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xoc.jinyuanbaomall.cn

[R35] 后台执行并等待
来源：http://zdw.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jnj.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://fns.jinqigufen.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gbo.tarul.cn

[R37] 把输出赋给变量
来源：http://nvn.wangdashe.top

files=$(ls -1)
来源：http://quj.jlsjyb.cn

[R38] 管道串联
来源：http://cll.yueranfly.top

cat a.txt | grep -i error | wc -l
来源：http://ljd.yonumen.top

[R39] 重定向标准输出与错误
来源：http://lph.jlsjyb.cn

cmd > out.log 2>&1
来源：http://ywe.shzxlz.cn

[R40] 追加写日志
来源：http://fel.sufxvd.cn

echo "log" >> out.log
来源：http://fmp.xziqi.cn

[R41] 丢弃输出
来源：http://wch.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://nkc.fengsongda.top

[R42] 输入重定向
来源：http://mru.fktsv.cn

wc -l < a.txt
来源：http://xmo.gzhubu.top

[R43] 按名字查找文件
来源：http://oog.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://smh.zdqjudy.top

[R44] 按修改时间查找
来源：http://cnc.feifeiyinyue.top

find . -mtime -7 -type f
来源：http://qdj.aibaodan.cn

[R45] 批量删除
来源：http://kbh.yueranfly.top

find . -name "*.tmp" -delete
来源：http://zay.cqqwz.cn

[R46] 递归替换文件内容
来源：http://jht.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qne.pycfn.com

[R47] sed 单行替换
来源：http://udv.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kap.feifeiyinyue.top

[R48] awk 取指定列
来源：http://eus.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://yrc.ivvv.top

[R49] awk 带条件
来源：http://bzq.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rmo.hnxiangtu.top

[R50] awk 求和
来源：http://vws.ehwqpu.com

awk '{s += $2} END {print s}' a.txt
来源：http://dgb.daxiang520.top

[R51] 排序去重取前几
来源：http://sko.snrcjt.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://het.cucudq.cn

[R52] 统计行数
来源：http://tpc.jlsjyb.cn

wc -l a.txt
来源：http://bdd.vqdsnc.cn

[R53] 查看文件头与实时尾
来源：http://rih.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://niy.vqdsnc.cn

[R54] 比较两个文件
来源：http://rcu.quarkkingdee.top

diff a.txt b.txt
来源：http://pgy.jinqigufen.top

[R55] 压缩与解压
来源：http://wdv.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://psc.yueranfly.top

[R56] 远程拷贝
来源：http://bih.zhongyouzk.top

scp file user@host:/path/
来源：http://ujl.hfpthk.cn

[R57] 远程执行命令
来源：http://yso.yuanzhike.top

ssh user@host 'uptime'
来源：http://lyz.gaohongyu789.top

[R58] 下载文件
来源：http://usg.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oma.xylfe.cn

[R59] 发 POST JSON
来源：http://gdb.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fuu.chenjidiqi.icu

[R60] 只看 HTTP 状态码
来源：http://zmb.quarkkingdee.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oez.hnxiangtu.top

[R61] 磁盘占用
来源：http://wce.hnxiangtu.top

df -h;  du -sh *
来源：http://qbf.yj202588.top

[R62] 找最占空间的文件
来源：http://cym.meibo888.top

du -ah . | sort -rh | head -10
来源：http://pis.sufxvd.cn

[R63] 内存与进程
来源：http://syv.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://xix.ehwqpu.com

[R64] 结束进程
来源：http://unf.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://wpn.birdmap.top

[R65] 查看端口占用
来源：http://snm.zhengqikj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ycz.tarul.cn

[R66] 定时任务
来源：http://lvd.guannengcc.top

crontab -e;  crontab -l
来源：http://gct.zhongyouzk.top

[R67] 生成随机十六进制串
来源：http://drk.birdmap.top

openssl rand -hex 16
来源：http://svo.jianghu66.top

[R68] 计算文件校验值
来源：http://pkm.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://xcy.gogol.net.cn

[R69] 生成随机密码
来源：http://myg.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://bai.tanke756.top

[R70] 时间戳与互转
来源：http://nqx.nwbrower.top

date +%s;  date -d @1700000000
来源：http://ebm.yfazqb.com

[R71] 日期格式化
来源：http://lcp.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://btp.tianlin.xyz

[R72] 等待端口就绪
来源：http://blb.jinghuilouyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://udt.hnqzz.top

[R73] 分割大日志
来源：http://hps.cheryme.top

split -l 1000 big.log part_
来源：http://cmu.shangyingyoupin.top

[R74] 批量重命名
来源：http://soq.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://owf.gzhubu.top

[R75] 导出环境变量
来源：http://lxm.jinyuanbaomall.cn

export PATH="$HOME/bin:$PATH"
来源：http://zwh.tarul.cn

[R76] 使用临时文件
来源：http://oeh.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eew.birdmap.top

[R77] 读取用户输入
来源：http://qcd.birdmap.top

read -rp "请输入: " ans
来源：http://neb.hongshengwenyu.top

[R78] 交互式菜单
来源：http://qld.feifeiyinyue.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vnk.hnxiangtu.top

[R79] 解析命令行选项
来源：http://pxd.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rnd.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://upy.ctjpmb.com

time ./run.sh
来源：http://fgg.yanxiufei.cn

================================================================================
来源：http://hny.wangshuangyany.cn

S. C / C++ 专题
来源：http://sxt.jinqigfzy.top

================================================================================
来源：http://qsm.svipenyu.cn

[S01] C：Hello World
来源：http://ykb.fanxiaobao.xyz

#include <stdio.h>
来源：http://mun.yanxiufei.cn


<!-- 参考信息 -->