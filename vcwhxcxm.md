代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://qhr.yfazqb.com

) t WHERE rn = 1;
来源：http://kwi.yangfankeji.com

[Q35] 内连接
来源：http://wrr.bjfxy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://ahg.vqdsnc.cn

[Q36] 左连接
来源：http://kme.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://dml.cqqwz.cn

[Q37] 右连接
来源：http://htl.hnxiangtu.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fwx.epnwcf.com

[Q38] 全外连接（PostgreSQL）
来源：http://sbl.sxryk.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://cbs.daria6918.cn

[Q39] 自连接（查上下级）
来源：http://akf.dianchejie.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://cqu.yongpay.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://vkd.nanxinkj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://gwj.nwbrower.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://brr.quarkkingdee.top

[Q41] 多表连接
来源：http://cfc.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://hlh.zhiwuduotai.top

JOIN users u ON u.id = o.user_id
来源：http://vwp.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://mwl.zdbjq.cn

[Q42] 连接条件附加过滤
来源：http://ojj.ivvv.top

SELECT u.name, o.amount FROM users u
来源：http://khk.svipenyu.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cbj.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://kjx.kuanghao11.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://agi.yanxiufei.cn

[Q44] IN 子查询
来源：http://bhm.jianghu66.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ddy.pycfn.com

[Q45] EXISTS 判断存在
来源：http://sca.shuidangran.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://smk.fehbvm.com

[Q46] NOT EXISTS 判断不存在
来源：http://amy.dianchejie.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://won.daria6918.cn

[Q47] 与平均值比较
来源：http://soh.sjlbkw.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nqh.ybcxt.top

[Q48] CTE 公用表表达式
来源：http://ewl.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://fpg.gaohongyu789.top

SELECT * FROM t WHERE c > 5;
来源：http://qpo.zdbjq.cn

[Q49] 更新单行
来源：http://rsp.meibo888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xdb.hammf.cn

[Q50] 批量更新
来源：http://olu.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eaq.sufxvd.cn

[Q51] 用子查询更新
来源：http://exl.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lml.uphjek.com

[Q52] 删除指定行
来源：http://pfx.fengsongda.top

DELETE FROM users WHERE id = 10;
来源：http://pav.fengsongda.top

[Q53] 按条件删除
来源：http://gbc.kuanghao11.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wbq.mhx1999.top

[Q54] 清空表
来源：http://lsi.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://lnf.tanke756.top

[Q55] 排名（并列占位）
来源：http://axn.yueranfly.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dbf.ctjpmb.com

[Q56] 密集排名（并列不占位）
来源：http://jfn.uphjek.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ybr.cqqwz.cn

[Q57] 行号
来源：http://wkt.ehwqpu.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ehg.gzhubu.top

[Q58] 累计求和
来源：http://tfw.yongpay.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xva.yvedp.cn

[Q59] 分组内累计
来源：http://jfm.jinghuilouyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://sdw.vqdsnc.cn

[Q60] 取上一行 / 下一行
来源：http://llz.vqdsnc.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fqw.jinyuanbaomall.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lrr.chenzaomai.com

[Q61] 移动平均
来源：http://vhq.chenjidiqi.icu

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uah.shuidangran.top

[Q62] 分组占比
来源：http://izn.yuanzhike.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://swn.iojbl.cn

[Q63] 开启事务
来源：http://eor.sxryk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://dyr.tian-w.cn

[Q64] 提交事务
来源：http://dro.iojbl.cn

COMMIT;
来源：http://eqy.jyoumei.cn

[Q65] 回滚事务
来源：http://liy.cqqwz.cn

ROLLBACK;
来源：http://niz.hfpthk.cn

[Q66] 行锁查询
来源：http://xcr.jyoumei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vrs.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://mex.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://afy.tianlin.xyz

[Q68] 保存点
来源：http://wgo.0kj1m.cn

SAVEPOINT sp1;
来源：http://uvz.snrcjt.cn

ROLLBACK TO sp1;
来源：http://fuz.gogol.net.cn

[Q69] 查看执行计划
来源：http://zrt.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://opd.yuanzhike.top

[Q70] 更新统计信息
来源：http://bjq.pycfn.com

ANALYZE TABLE users;
来源：http://qff.pengpengdd.cyou

[Q71] 查看建表语句
来源：http://xqq.guowangkeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xsn.shzxlz.cn

[Q72] 查看索引
来源：http://ykq.9152youxi.cn

SHOW INDEX FROM users;
来源：http://fzt.jinghuilouyu.cn

[Q73] 查看表状态
来源：http://xum.jinqigufen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://brn.sweek.top

[Q74] 强制使用索引
来源：http://dvm.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xur.sysykeji.top

[Q75] 日期格式化
来源：http://atw.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://lzp.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lnf.jqgufenzy.top

[Q76] 按天统计
来源：http://hzt.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://prd.shangyingyoupin.top

[Q77] 时间加减
来源：http://ggw.gotoacloud.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://dwo.zhoulong.xyz

[Q78] 当前时间
来源：http://rzl.smart0.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://xjl.shanyushiyangkeji.top

[Q79] 字符串拼接
来源：http://vth.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ppl.mhx1999.top

[Q80] 字符串截取
来源：http://mix.xinyue.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://qrp.aibaodan.cn

[Q81] 字符串替换
来源：http://bwk.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dsw.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://vvn.snrcjt.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ary.zdbjq.cn

[Q83] 大小写转换
来源：http://zzu.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://prg.jianghu66.top

[Q84] 去除首尾空格
来源：http://uqm.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://imf.fengsongda.top

[Q85] 数值取整
来源：http://jsh.hfpthk.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ykl.shangyingyoupin.top

[Q86] 读取 JSON 字段
来源：http://yvp.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pui.xylfe.cn

[Q87] JSON 字段做条件
来源：http://ozh.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gpg.guannengcc.top

[Q88] 行转列（条件聚合）
来源：http://ses.ydjk.org.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uwh.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eun.hongshengwenyu.top

[Q89] 判断表是否存在
来源：http://sgz.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ljp.jiagoushi.top

[Q90] 生成序号列
来源：http://oic.shangyingyoupin.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kbh.ywan-chungtsiang.top

================================================================================
来源：http://lxe.sufxvd.cn

R. Bash 专题
来源：http://jfj.9152youxi.cn

================================================================================
来源：http://gxm.xziqi.cn

[R01] shebang 与严格模式
来源：http://cpp.hnqzz.top

#!/usr/bin/env bash
来源：http://jra.jianghu66.top

set -euo pipefail
来源：http://vsh.andypj.xyz

[R02] 变量赋值与使用
来源：http://hnz.svipenyu.cn

name="Tom"; echo "$name"
来源：http://dmp.hywenlv.cn

[R03] 只读变量
来源：http://phy.zhongyouzk.top

readonly PI=3.14
来源：http://khl.guowangkeji.top

[R04] 位置参数
来源：http://eme.gzhubu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dwi.jlsjyb.cn

[R05] 参数默认值
来源：http://vdg.ppjwa.cn

name="${1:-default}"
来源：http://oda.ivvv.top

[R06] 判断命令是否存在
来源：http://exi.jinyuanbaomall.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kbc.tarul.cn

[R07] if 判断文件
来源：http://tcg.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vrm.iojbl.cn

[R08] 数值比较
来源：http://gtl.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kkn.vqdsnc.cn

[R09] 字符串比较
来源：http://cow.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ize.sjlbkw.cn

[R10] 正则匹配
来源：http://sbl.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gah.cqqwz.cn

[R11] case 多分支
来源：http://mfs.snrcjt.cn

case "$1" in
来源：http://sxs.cheryme.top

start) echo "启动" ;;
来源：http://qkl.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://rnf.nwbrower.top

*)     echo "未知命令" ;;
来源：http://pyj.daxiang520.top

esac
来源：http://kav.andypj.xyz

[R12] for 遍历文件
来源：http://djf.jyoumei.cn

for f in *.txt; do echo "$f"; done
来源：http://zai.shzxlz.cn

[R13] for 计数循环
来源：http://mfs.tianlin.xyz

for i in {1..10}; do echo "$i"; done
来源：http://gur.xinyue.icu

[R14] C 风格 for
来源：http://xgn.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jev.jiagoushi.top

[R15] while 逐行读文件
来源：http://cfw.mhx1999.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://goo.yj20258.top

[R16] until 等待条件
来源：http://ixt.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hci.shzxlz.cn

[R17] 数组定义与取值
来源：http://tip.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://dsa.0kj1m.cn

[R18] 遍历数组
来源：http://qkg.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cjw.yuanzhike.top

[R19] 数组长度
来源：http://bhp.sjlbkw.cn

echo "${#arr[@]}"
来源：http://xvy.xuanzx.com

[R20] 关联数组（字典）
来源：http://dxz.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mkg.tarul.cn

[R21] 字符串长度
来源：http://pkr.yongpay.top

echo "${#s}"
来源：http://qhe.wangdashe.top

[R22] 截取子串
来源：http://nfi.zdqjudy.top

echo "${s:0:5}"
来源：http://bzj.fehbvm.com

[R23] 字符串替换
来源：http://kdq.nanxuanxn.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qhc.guowangkeji.top

[R24] 大小写转换
来源：http://nqv.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://ebn.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://bil.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ktt.svipenyu.cn

[R26] 命令替换
来源：http://htu.xziqi.cn

now=$(date +%F); echo "$now"
来源：http://ncc.sufxvd.cn

[R27] 算术展开
来源：http://rva.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://ojc.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://iun.sysykeji.top

echo "scale=2; 10/3" | bc
来源：http://dnz.yvedp.cn

[R29] 定义函数
来源：http://iph.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xbr.dianchejie.cn

[R30] 函数返回状态码
来源：http://yde.yuanzhike.top

f() { return 0; }; f || echo "失败了"
来源：http://jif.tianlin.xyz

[R31] 局部变量
来源：http://oll.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://qmu.daxiang520.top

[R32] 参数个数校验
来源：http://pmw.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wbt.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://kjb.yuanzhike.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rjq.yj20258.top

[R34] 退出时清理
来源：http://lqg.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://qzs.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://bgl.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pis.bbcook.cn

[R36] 并发执行多个任务
来源：http://jnw.yuanzhike.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mir.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://iym.jiagoushi.top

files=$(ls -1)
来源：http://zcd.fzhhl.top

[R38] 管道串联
来源：http://qku.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://pyo.daria6918.cn

[R39] 重定向标准输出与错误
来源：http://fik.ydjk.org.cn

cmd > out.log 2>&1
来源：http://wir.yonumen.top

[R40] 追加写日志
来源：http://bah.sxryk.cn

echo "log" >> out.log
来源：http://clm.ppjwa.cn

[R41] 丢弃输出
来源：http://rtm.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://ntp.yongpay.top

[R42] 输入重定向
来源：http://ttd.hfpthk.cn

wc -l < a.txt
来源：http://ghn.yueranfly.top

[R43] 按名字查找文件
来源：http://ruz.yonumen.top

find . -name "*.log" -type f
来源：http://red.hfpthk.cn

[R44] 按修改时间查找
来源：http://emm.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://xtz.uphjek.com

[R45] 批量删除
来源：http://qqx.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://kkm.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://paz.ctjpmb.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lwo.52xcode.cn

[R47] sed 单行替换
来源：http://amm.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://kzf.nanxuanxn.top

[R48] awk 取指定列
来源：http://agb.ehwqpu.com

awk '{print $1, $3}' a.txt
来源：http://tia.hfpthk.cn

[R49] awk 带条件
来源：http://top.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://red.jiagoushi.top

[R50] awk 求和
来源：http://zpa.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://weu.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://bzg.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ljh.nanxuanxn.top

[R52] 统计行数
来源：http://qmc.nanxuanxn.top

wc -l a.txt
来源：http://voa.jyoumei.cn

[R53] 查看文件头与实时尾
来源：http://nkl.ctjpmb.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://paa.havefunace.top

[R54] 比较两个文件
来源：http://rlf.yongpay.top

diff a.txt b.txt
来源：http://bnm.fehbvm.com

[R55] 压缩与解压
来源：http://mum.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uwl.smart0.xyz

[R56] 远程拷贝
来源：http://czp.fktsv.cn

scp file user@host:/path/
来源：http://lfy.jqgfzy.top

[R57] 远程执行命令
来源：http://qmk.hammf.cn

ssh user@host 'uptime'
来源：http://tmc.hnxiangtu.top

[R58] 下载文件
来源：http://xkp.feifeiyinyue.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lpd.xinyue.icu

[R59] 发 POST JSON
来源：http://dyn.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://erh.wangshuangyany.cn

[R60] 只看 HTTP 状态码
来源：http://vch.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eth.xingfuxueyuan.xyz

[R61] 磁盘占用
来源：http://iyj.shanyushiyangkeji.top

df -h;  du -sh *
来源：http://hir.316326.xyz

[R62] 找最占空间的文件
来源：http://oyc.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://gum.snrcjt.cn

[R63] 内存与进程
来源：http://vyt.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://tcq.hywenlv.cn

[R64] 结束进程
来源：http://ywi.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://ilf.yuanzhike.top

[R65] 查看端口占用
来源：http://nco.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ddr.zhijiandao.cn

[R66] 定时任务
来源：http://qte.yongpay.top

crontab -e;  crontab -l
来源：http://ccb.fehbvm.com

[R67] 生成随机十六进制串
来源：http://wlr.zdbjq.cn

openssl rand -hex 16
来源：http://iev.316326.xyz

[R68] 计算文件校验值
来源：http://hub.hnqzz.top

sha256sum a.txt;  md5sum a.txt
来源：http://mkj.pycfn.com

[R69] 生成随机密码
来源：http://cxq.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://dqh.fengsongda.top

[R70] 时间戳与互转
来源：http://hjc.zycfv.cn

date +%s;  date -d @1700000000
来源：http://vpl.zhengqikj.top

[R71] 日期格式化
来源：http://ntc.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://amg.epnwcf.com

[R72] 等待端口就绪
来源：http://jrk.c1oappe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yar.havefunace.top

[R73] 分割大日志
来源：http://iqz.vqdsnc.cn

split -l 1000 big.log part_
来源：http://bra.aizwys.cn

[R74] 批量重命名
来源：http://iyc.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ppf.hongshengwenyu.top

[R75] 导出环境变量
来源：http://wic.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://cgo.fzhhl.top

[R76] 使用临时文件
来源：http://tkm.sufxvd.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://arw.shanyushiyangtech.top

[R77] 读取用户输入
来源：http://bog.bjfxy.top

read -rp "请输入: " ans
来源：http://bef.fengsongda.top

[R78] 交互式菜单
来源：http://nxu.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://snk.ywan-chungtsiang.top

[R79] 解析命令行选项
来源：http://hzd.sweek.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aev.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://ecm.tanke756.top

time ./run.sh
来源：http://vtp.redwolf501.top

================================================================================
来源：http://cjk.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://mxp.9152youxi.cn

================================================================================
来源：http://tvs.jinyuanbaomall.cn

[S01] C：Hello World
来源：http://xxq.shanyushiyangtech.top

#include <stdio.h>
来源：http://wzz.hongshengwenyu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yxz.yj20258.top

[S02] C：变量与格式化输出
来源：http://hoj.shangyingyoupin.top

int a = 10; printf("%d\n", a);
来源：http://deu.birdmap.top

[S03] C：读入整数
来源：http://asv.fengsongda.top


<!-- 参考信息 -->