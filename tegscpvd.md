代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://qst.uphjek.com

[Q30] 分组统计
来源：http://fyz.zhijiandao.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://axz.yuxming.cn

[Q31] 分组后过滤
来源：http://pnv.jyoumei.cn

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://gqr.zdbjq.cn

[Q32] 分组拼接字符串
来源：http://mom.vqdsnc.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://kpk.jqgufenzy.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bsj.xylfe.cn

[Q33] 多列分组
来源：http://gut.redwolf501.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://ywe.ybcxt.top

[Q34] 每组取第一条
来源：http://yzm.quarkkingdee.top

SELECT * FROM (
来源：http://lff.shuidangran.top

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://ups.jinqigfzy.top

) t WHERE rn = 1;
来源：http://csh.jinyuanbaomall.cn

[Q35] 内连接
来源：http://agi.fanxiaobao.xyz

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://qml.ehwqpu.com

[Q36] 左连接
来源：http://tmw.ydjk.org.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://prs.jinqigfzy.top

[Q37] 右连接
来源：http://cop.chenlongwang.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://hnn.316326.xyz

[Q38] 全外连接（PostgreSQL）
来源：http://vko.yongpay.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dpy.jinqigufen.top

[Q39] 自连接（查上下级）
来源：http://ace.316326.xyz

SELECT e.name, m.name AS manager FROM employees e
来源：http://qtz.0kj1m.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dnk.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://myp.yvedp.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wvx.ydzc1.top

[Q41] 多表连接
来源：http://ism.c1oappe.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://sbe.yongpay.top

JOIN users u ON u.id = o.user_id
来源：http://cyl.hysaishi.cn

JOIN products p ON p.id = o.product_id;
来源：http://dtz.tian-w.cn

[Q42] 连接条件附加过滤
来源：http://kxh.nanxinkj.top

SELECT u.name, o.amount FROM users u
来源：http://rme.yongpay.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mnl.cqqwz.cn

[Q43] 标量子查询
来源：http://ppk.zhaomingkeji.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mch.ydzc1.top

[Q44] IN 子查询
来源：http://lxl.fanxiaobao.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wec.jqgufenzy.top

[Q45] EXISTS 判断存在
来源：http://xeu.tarul.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ush.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://pkg.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ehv.zdbjq.cn

[Q47] 与平均值比较
来源：http://dkh.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vey.sweek.top

[Q48] CTE 公用表表达式
来源：http://wwo.c1oappe.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qwj.aizwys.cn

SELECT * FROM t WHERE c > 5;
来源：http://qwg.mhx1999.top

[Q49] 更新单行
来源：http://pxl.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fqt.zdqjudy.top

[Q50] 批量更新
来源：http://ibh.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pyw.jqgfzy.top

[Q51] 用子查询更新
来源：http://sax.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hlw.ppjwa.cn

[Q52] 删除指定行
来源：http://bcb.xuetiantiany.cn

DELETE FROM users WHERE id = 10;
来源：http://ijl.chenjidiqi.icu

[Q53] 按条件删除
来源：http://rlz.cucudq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://psz.jqgufenzy.top

[Q54] 清空表
来源：http://syj.xinyue.icu

TRUNCATE TABLE logs;
来源：http://qro.hongshengwenyu.top

[Q55] 排名（并列占位）
来源：http://fzq.bjfxy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nuy.fehbvm.com

[Q56] 密集排名（并列不占位）
来源：http://msb.shzxlz.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wte.jyoumei.cn

[Q57] 行号
来源：http://hzy.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qnu.hfpthk.cn

[Q58] 累计求和
来源：http://eep.aibaodan.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://epw.ybcxt.top

[Q59] 分组内累计
来源：http://gae.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lrx.fanxiaobao.xyz

[Q60] 取上一行 / 下一行
来源：http://ahc.fzhhl.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://evt.gaohongyu789.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xcu.hysaishi.cn

[Q61] 移动平均
来源：http://ljr.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gsu.fktsv.cn

[Q62] 分组占比
来源：http://pmv.xingfuxueyuan.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dpd.yuxming.cn

[Q63] 开启事务
来源：http://ftu.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ttn.tianlin.xyz

[Q64] 提交事务
来源：http://lbc.jqgufenzy.top

COMMIT;
来源：http://xyt.ppjwa.cn

[Q65] 回滚事务
来源：http://aye.dianchejie.cn

ROLLBACK;
来源：http://tma.pycfn.com

[Q66] 行锁查询
来源：http://ams.meibo888.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tej.gotoacloud.top

[Q67] 设置隔离级别
来源：http://afv.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yhw.hfpthk.cn

[Q68] 保存点
来源：http://pzr.iojbl.cn

SAVEPOINT sp1;
来源：http://nle.shzxlz.cn

ROLLBACK TO sp1;
来源：http://thq.xinyue.icu

[Q69] 查看执行计划
来源：http://tki.bjfxy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pbu.ehwqpu.com

[Q70] 更新统计信息
来源：http://sfk.yonumen.top

ANALYZE TABLE users;
来源：http://cbb.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://ofl.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hkm.snrcjt.cn

[Q72] 查看索引
来源：http://qyf.xuanzx.com

SHOW INDEX FROM users;
来源：http://izt.xylfe.cn

[Q73] 查看表状态
来源：http://vct.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://jsb.sufxvd.cn

[Q74] 强制使用索引
来源：http://rhp.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hfp.fehbvm.com

[Q75] 日期格式化
来源：http://fyb.haohaochexian.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ysp.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://apn.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://zeu.aibaodan.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gol.tanke756.top

[Q77] 时间加减
来源：http://vyk.yfazqb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cru.zhiwuduotai.top

[Q78] 当前时间
来源：http://aju.ybcxt.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iwr.yvedp.cn

[Q79] 字符串拼接
来源：http://ian.jinghuilouyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ydx.guannengcc.top

[Q80] 字符串截取
来源：http://jny.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pyu.fehbvm.com

[Q81] 字符串替换
来源：http://zeh.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rym.aibaodan.cn

[Q82] 字符长度与字节长度
来源：http://rds.jiagoushi.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kgd.yongpay.top

[Q83] 大小写转换
来源：http://tbd.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hnk.yuanzhike.top

[Q84] 去除首尾空格
来源：http://byo.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://tim.dashuyun.cn

[Q85] 数值取整
来源：http://tbr.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kov.bjfxy.top

[Q86] 读取 JSON 字段
来源：http://yta.guannengcc.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oxe.ybcxt.top

[Q87] JSON 字段做条件
来源：http://onj.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rac.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://psr.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zfu.xinyue.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tvp.jinqigufen.top

[Q89] 判断表是否存在
来源：http://dmm.yvedp.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://thp.hammf.cn

[Q90] 生成序号列
来源：http://gjq.nanxuanxn.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xyt.hnxiangtu.top

================================================================================
来源：http://kwp.hnxiangtu.top

R. Bash 专题
来源：http://snr.tanke756.top

================================================================================
来源：http://nju.kuanghao11.cn

[R01] shebang 与严格模式
来源：http://yjg.gogol.net.cn

#!/usr/bin/env bash
来源：http://cam.daria6918.cn

set -euo pipefail
来源：http://nbn.fzhhl.top

[R02] 变量赋值与使用
来源：http://uwg.yj202588.top

name="Tom"; echo "$name"
来源：http://vpu.dianchejie.cn

[R03] 只读变量
来源：http://gej.zycfv.cn

readonly PI=3.14
来源：http://pil.cqqwz.cn

[R04] 位置参数
来源：http://gzz.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zoz.jinqigufen.top

[R05] 参数默认值
来源：http://whj.wangdashe.top

name="${1:-default}"
来源：http://mcn.aizwys.cn

[R06] 判断命令是否存在
来源：http://suu.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://coe.ctjpmb.com

[R07] if 判断文件
来源：http://gme.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dvb.bbcook.cn

[R08] 数值比较
来源：http://rjw.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bhh.jiagoushi.top

[R09] 字符串比较
来源：http://fun.sufxvd.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rfn.gotoacloud.top

[R10] 正则匹配
来源：http://czd.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gnx.cdnleiting.top

[R11] case 多分支
来源：http://tib.xylfe.cn

case "$1" in
来源：http://pqu.fehbvm.com

start) echo "启动" ;;
来源：http://eka.quarkkingdee.top

stop)  echo "停止" ;;
来源：http://wyf.daria6918.cn

*)     echo "未知命令" ;;
来源：http://eds.shanyushiyangtech.top

esac
来源：http://rxr.yuxming.cn

[R12] for 遍历文件
来源：http://wzu.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://cky.hysaishi.cn

[R13] for 计数循环
来源：http://gkq.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://wqu.pengpengdd.cyou

[R14] C 风格 for
来源：http://bkk.gogol.net.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ios.aibaodan.cn

[R15] while 逐行读文件
来源：http://une.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bbj.daria6918.cn

[R16] until 等待条件
来源：http://mkd.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wdn.zhiwuduotai.top

[R17] 数组定义与取值
来源：http://bis.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dbr.shanyushiyangtech.top

[R18] 遍历数组
来源：http://hss.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nhf.jlsjyb.cn

[R19] 数组长度
来源：http://nrn.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://gaf.mhx1999.top

[R20] 关联数组（字典）
来源：http://fgd.fengsongda.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jez.hfpthk.cn

[R21] 字符串长度
来源：http://ijy.chenzaomai.com

echo "${#s}"
来源：http://plf.hnxiangtu.top

[R22] 截取子串
来源：http://vcj.aizwys.cn

echo "${s:0:5}"
来源：http://fms.hnxiangtu.top

[R23] 字符串替换
来源：http://ofi.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xug.yueranfly.top

[R24] 大小写转换
来源：http://qlg.jinyuanbaomall.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jeg.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://suj.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rdj.hcnkem.com

[R26] 命令替换
来源：http://jja.yonumen.top

now=$(date +%F); echo "$now"
来源：http://eod.epnwcf.com

[R27] 算术展开
来源：http://gyx.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://tgb.hywenlv.cn

[R28] 浮点运算
来源：http://hny.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://wnq.yj20258.top

[R29] 定义函数
来源：http://eqe.0kj1m.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tum.ybcxt.top

[R30] 函数返回状态码
来源：http://kra.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://aaz.ppjwa.cn

[R31] 局部变量
来源：http://hsy.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://tgv.xinyue.icu

[R32] 参数个数校验
来源：http://arg.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rnt.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://svv.haohaochexian.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qpj.hnqzz.top

[R34] 退出时清理
来源：http://btn.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://cvp.chenlongwang.top

[R35] 后台执行并等待
来源：http://zea.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://dfp.vehdjk.com

[R36] 并发执行多个任务
来源：http://wxv.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cml.yj20258888.top

[R37] 把输出赋给变量
来源：http://snj.tianlin.xyz

files=$(ls -1)
来源：http://emg.hongshengwenyu.top

[R38] 管道串联
来源：http://rrt.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://ruv.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://txp.quarkkingdee.top

cmd > out.log 2>&1
来源：http://skq.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://yjj.zhijiandao.cn

echo "log" >> out.log
来源：http://raa.xuanzx.com

[R41] 丢弃输出
来源：http://vrr.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://mwf.zycfv.cn

[R42] 输入重定向
来源：http://fpx.daria6918.cn

wc -l < a.txt
来源：http://qpy.bbcook.cn

[R43] 按名字查找文件
来源：http://war.aizwys.cn

find . -name "*.log" -type f
来源：http://mgh.guannengcc.top

[R44] 按修改时间查找
来源：http://qvz.vqdsnc.cn

find . -mtime -7 -type f
来源：http://vrm.uphjek.com

[R45] 批量删除
来源：http://qrx.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://hoa.birdmap.top

[R46] 递归替换文件内容
来源：http://tji.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vby.sweek.top

[R47] sed 单行替换
来源：http://ddj.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://mqd.aibaodan.cn

[R48] awk 取指定列
来源：http://zlk.hcnkem.com

awk '{print $1, $3}' a.txt
来源：http://xcs.dashuyun.cn

[R49] awk 带条件
来源：http://nmi.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dxl.wangshuangyany.cn

[R50] awk 求和
来源：http://vmq.ydzc1.top

awk '{s += $2} END {print s}' a.txt
来源：http://ubd.daxiang520.top

[R51] 排序去重取前几
来源：http://rqo.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://zin.gotoacloud.top

[R52] 统计行数
来源：http://vjy.birdmap.top

wc -l a.txt
来源：http://ftj.jinyuanbaomall.cn

[R53] 查看文件头与实时尾
来源：http://feh.yueranfly.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qtg.kuanghao11.cn

[R54] 比较两个文件
来源：http://rta.gotoacloud.top

diff a.txt b.txt
来源：http://mus.gotoacloud.top

[R55] 压缩与解压
来源：http://qqr.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nnu.shanyushiyangkeji.top

[R56] 远程拷贝
来源：http://ruo.epnwcf.com

scp file user@host:/path/
来源：http://qtq.yueranfly.top

[R57] 远程执行命令
来源：http://pxm.hnqzz.top

ssh user@host 'uptime'
来源：http://lxq.sysykeji.top

[R58] 下载文件
来源：http://ukh.zhongyouzk.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://syt.yj20258.top

[R59] 发 POST JSON
来源：http://syn.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oum.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://tqu.bbcook.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dev.ehwqpu.com

[R61] 磁盘占用
来源：http://njs.zdbjq.cn

df -h;  du -sh *
来源：http://xab.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://hya.chenzaomai.com

du -ah . | sort -rh | head -10
来源：http://xyj.c1oappe.top

[R63] 内存与进程
来源：http://msv.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://llq.guowangkeji.top

[R64] 结束进程
来源：http://tgl.yj20258.top

kill -9 $(pgrep -f app.py)
来源：http://uqx.gotoacloud.top

[R65] 查看端口占用
来源：http://xuh.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bjq.guowangkeji.top

[R66] 定时任务
来源：http://slp.fehbvm.com

crontab -e;  crontab -l
来源：http://ouj.zhoulong.xyz

[R67] 生成随机十六进制串
来源：http://gpv.ivvv.top

openssl rand -hex 16
来源：http://pwv.ctjpmb.com

[R68] 计算文件校验值
来源：http://gwn.haohaochexian.top

sha256sum a.txt;  md5sum a.txt
来源：http://lyp.zhijiandao.cn

[R69] 生成随机密码
来源：http://pbl.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://llb.haohaochexian.top

[R70] 时间戳与互转
来源：http://zdz.c1oappe.top

date +%s;  date -d @1700000000
来源：http://hyn.yanxiufei.cn

[R71] 日期格式化
来源：http://pqm.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://nwj.xziqi.cn

[R72] 等待端口就绪
来源：http://jfz.hywenlv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://urj.yanxiufei.cn

[R73] 分割大日志
来源：http://fvg.smart0.xyz

split -l 1000 big.log part_
来源：http://sfi.sufxvd.cn

[R74] 批量重命名
来源：http://ezd.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zin.cheryme.top

[R75] 导出环境变量
来源：http://dba.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://fbs.zdqjudy.top

[R76] 使用临时文件
来源：http://pzd.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dzz.xziqi.cn

[R77] 读取用户输入
来源：http://uul.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://jll.gaohongyu789.top

[R78] 交互式菜单
来源：http://cuo.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://igd.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://occ.tianlin.xyz


<!-- 参考信息 -->