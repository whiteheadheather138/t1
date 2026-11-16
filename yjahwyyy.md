代发 wailian999

[Q36] 左连接
来源：http://ozn.nwbrower.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wiw.aizwys.cn

[Q37] 右连接
来源：http://kvy.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cvf.hnqzz.top

[Q38] 全外连接（PostgreSQL）
来源：http://uve.hnqzz.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://pki.ctjpmb.com

[Q39] 自连接（查上下级）
来源：http://akw.yanxiufei.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://eok.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://tkb.gogol.net.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mxb.fzhhl.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://qlh.yangfankeji.com

[Q41] 多表连接
来源：http://dxp.ppjwa.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://rte.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://dkz.redwolf501.top

JOIN products p ON p.id = o.product_id;
来源：http://din.chenlongwang.top

[Q42] 连接条件附加过滤
来源：http://xpd.cdnleiting.top

SELECT u.name, o.amount FROM users u
来源：http://jzr.316326.xyz

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ewv.yj20258888.top

[Q43] 标量子查询
来源：http://kdr.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rwy.wangshuangyany.cn

[Q44] IN 子查询
来源：http://bts.feifeiyinyue.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wrk.mhx1999.top

[Q45] EXISTS 判断存在
来源：http://ydy.epnwcf.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nsu.yangfankeji.com

[Q46] NOT EXISTS 判断不存在
来源：http://iwd.fktsv.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://khv.hongshengwenyu.top

[Q47] 与平均值比较
来源：http://lzz.tianlin.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://sro.havefunace.top

[Q48] CTE 公用表表达式
来源：http://axf.shzxlz.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://etu.shzxlz.cn

SELECT * FROM t WHERE c > 5;
来源：http://mft.zhiwuduotai.top

[Q49] 更新单行
来源：http://ciu.ivvv.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://afl.hnxiangtu.top

[Q50] 批量更新
来源：http://iut.zhixingplan.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uwj.gaohongyu789.top

[Q51] 用子查询更新
来源：http://usi.gotoacloud.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jsh.xziqi.cn

[Q52] 删除指定行
来源：http://hlz.hesvh.cn

DELETE FROM users WHERE id = 10;
来源：http://wfc.xziqi.cn

[Q53] 按条件删除
来源：http://gjk.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://waf.vqdsnc.cn

[Q54] 清空表
来源：http://ixd.xuanzx.com

TRUNCATE TABLE logs;
来源：http://ewr.316326.xyz

[Q55] 排名（并列占位）
来源：http://mok.feifeiyinyue.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jxr.zhixingplan.top

[Q56] 密集排名（并列不占位）
来源：http://lfr.daxiang520.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xsd.ehwqpu.com

[Q57] 行号
来源：http://acq.gogol.net.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://znk.tianlin.xyz

[Q58] 累计求和
来源：http://kll.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jdi.iojbl.cn

[Q59] 分组内累计
来源：http://rcc.yangfankeji.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zmm.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://nym.bbcook.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jbw.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://add.hywenlv.cn

[Q61] 移动平均
来源：http://ywn.tian-w.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://oki.sjlbkw.cn

[Q62] 分组占比
来源：http://sdf.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://rbc.ivvv.top

[Q63] 开启事务
来源：http://dwk.shuidangran.top

START TRANSACTION;                -- 或 BEGIN
来源：http://xbj.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://dvw.c1oappe.top

COMMIT;
来源：http://pgv.chenlongwang.top

[Q65] 回滚事务
来源：http://cdq.tian-w.cn

ROLLBACK;
来源：http://hok.yj202588.top

[Q66] 行锁查询
来源：http://gxi.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gwc.tianlin.xyz

[Q67] 设置隔离级别
来源：http://iog.zhongyouzk.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kzc.52xcode.cn

[Q68] 保存点
来源：http://rit.smart0.xyz

SAVEPOINT sp1;
来源：http://wnc.hnqzz.top

ROLLBACK TO sp1;
来源：http://ozd.ydzc1.top

[Q69] 查看执行计划
来源：http://yhy.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xts.wangdashe.top

[Q70] 更新统计信息
来源：http://dzt.ctjpmb.com

ANALYZE TABLE users;
来源：http://ymb.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://mhn.jqgufenzy.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://osx.bbcook.cn

[Q72] 查看索引
来源：http://wnk.nanxuanxn.top

SHOW INDEX FROM users;
来源：http://jjb.dashuyun.cn

[Q73] 查看表状态
来源：http://itc.yangfankeji.com

SHOW TABLE STATUS LIKE 'users';
来源：http://khr.0kj1m.cn

[Q74] 强制使用索引
来源：http://sfe.feifeiyinyue.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hli.c1oappe.top

[Q75] 日期格式化
来源：http://ner.havefunace.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://anh.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jzu.meibo888.top

[Q76] 按天统计
来源：http://klq.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vqv.zhiwuduotai.top

[Q77] 时间加减
来源：http://dtm.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cdb.redwolf501.top

[Q78] 当前时间
来源：http://bkb.nanxuanxn.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vib.gotoacloud.top

[Q79] 字符串拼接
来源：http://bvs.jianghu66.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://fsk.tarul.cn

[Q80] 字符串截取
来源：http://ixy.chenzaomai.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yrs.cashguo.top

[Q81] 字符串替换
来源：http://gfl.havefunace.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://whg.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://ggn.fengsongda.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kxb.yj202588.top

[Q83] 大小写转换
来源：http://zbf.havefunace.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vky.sufxvd.cn

[Q84] 去除首尾空格
来源：http://jnd.aizwys.cn

SELECT TRIM(name) FROM users;
来源：http://pbz.yanxiufei.cn

[Q85] 数值取整
来源：http://qyu.nwbrower.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://elw.gogol.net.cn

[Q86] 读取 JSON 字段
来源：http://lxh.nanxuanxn.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://saj.gotoacloud.top

[Q87] JSON 字段做条件
来源：http://orc.feifeiyinyue.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ety.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://eum.52xcode.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zmk.dashuyun.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ovh.guannengcc.top

[Q89] 判断表是否存在
来源：http://hpb.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yjc.yj202588.top

[Q90] 生成序号列
来源：http://cyv.kuanghao11.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ksn.fanxiaobao.xyz

================================================================================
来源：http://jeu.nanxuanxn.top

R. Bash 专题
来源：http://eag.tarul.cn

================================================================================
来源：http://esr.yangfankeji.com

[R01] shebang 与严格模式
来源：http://vqe.birdmap.top

#!/usr/bin/env bash
来源：http://zgc.nanxinkj.top

set -euo pipefail
来源：http://xcj.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://xrm.yfazqb.com

name="Tom"; echo "$name"
来源：http://tax.ybcxt.top

[R03] 只读变量
来源：http://ykz.aibaodan.cn

readonly PI=3.14
来源：http://xlr.xylfe.cn

[R04] 位置参数
来源：http://ive.jinghuilouyu.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zzp.cqqwz.cn

[R05] 参数默认值
来源：http://wzp.aibaodan.cn

name="${1:-default}"
来源：http://yso.uphjek.com

[R06] 判断命令是否存在
来源：http://dcv.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oyu.ybcxt.top

[R07] if 判断文件
来源：http://gxb.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xpk.hnqzz.top

[R08] 数值比较
来源：http://fny.cdnleiting.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fqm.aibaodan.cn

[R09] 字符串比较
来源：http://wtw.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kld.dianchejie.cn

[R10] 正则匹配
来源：http://mtg.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pmw.jqgfzy.top

[R11] case 多分支
来源：http://jvq.yongpay.top

case "$1" in
来源：http://nmy.ppjwa.cn

start) echo "启动" ;;
来源：http://lpo.andypj.xyz

stop)  echo "停止" ;;
来源：http://but.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://uqr.yj20258888.top

esac
来源：http://dln.meibo888.top

[R12] for 遍历文件
来源：http://rbk.mhx1999.top

for f in *.txt; do echo "$f"; done
来源：http://pdu.yonumen.top

[R13] for 计数循环
来源：http://uxs.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://kes.svipenyu.cn

[R14] C 风格 for
来源：http://tkh.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://awz.zhixingplan.top

[R15] while 逐行读文件
来源：http://rpr.yanxiufei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lio.9152youxi.cn

[R16] until 等待条件
来源：http://jql.zhiwuduotai.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cjt.sysykeji.top

[R17] 数组定义与取值
来源：http://oel.nanxuanxn.top

arr=(a b c); echo "${arr[0]}"
来源：http://khu.hongshengwenyu.top

[R18] 遍历数组
来源：http://vjo.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bal.xinyue.icu

[R19] 数组长度
来源：http://jzx.quarkkingdee.top

echo "${#arr[@]}"
来源：http://jsl.zdqjudy.top

[R20] 关联数组（字典）
来源：http://qja.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gut.ybcxt.top

[R21] 字符串长度
来源：http://dhp.c1oappe.top

echo "${#s}"
来源：http://kps.vehdjk.com

[R22] 截取子串
来源：http://wvz.vehdjk.com

echo "${s:0:5}"
来源：http://cki.yuanzhike.top

[R23] 字符串替换
来源：http://cpx.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hte.ppjwa.cn

[R24] 大小写转换
来源：http://nzc.dashuyun.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lyx.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://hys.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://psx.iojbl.cn

[R26] 命令替换
来源：http://npt.feifeiyinyue.top

now=$(date +%F); echo "$now"
来源：http://xkc.uphjek.com

[R27] 算术展开
来源：http://qzz.haohaochexian.top

echo $((1 + 2 * 3))
来源：http://coe.guannengcc.top

[R28] 浮点运算
来源：http://rze.ywan-chungtsiang.top

echo "scale=2; 10/3" | bc
来源：http://bgh.shanyushiyangkeji.top

[R29] 定义函数
来源：http://tii.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qqr.jqgufenzy.top

[R30] 函数返回状态码
来源：http://jyb.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://dhp.hesvh.cn

[R31] 局部变量
来源：http://zjc.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://tzw.zdbjq.cn

[R32] 参数个数校验
来源：http://dup.52xcode.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tmi.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://pty.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://khn.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://tff.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://bal.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://lyt.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hsu.yonumen.top

[R36] 并发执行多个任务
来源：http://qbi.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dra.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://pwt.xuetiantiany.cn

files=$(ls -1)
来源：http://fcq.xylfe.cn

[R38] 管道串联
来源：http://sqc.wangdashe.top

cat a.txt | grep -i error | wc -l
来源：http://vxa.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://hmc.redwolf501.top

cmd > out.log 2>&1
来源：http://wfw.yfazqb.com

[R40] 追加写日志
来源：http://bdb.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://wec.tian-w.cn

[R41] 丢弃输出
来源：http://eui.gotoacloud.top

cmd >/dev/null 2>&1
来源：http://tck.wangdashe.top

[R42] 输入重定向
来源：http://fxc.redwolf501.top

wc -l < a.txt
来源：http://ipo.xziqi.cn

[R43] 按名字查找文件
来源：http://yxr.tian-w.cn

find . -name "*.log" -type f
来源：http://nlm.bbcook.cn

[R44] 按修改时间查找
来源：http://kcr.bjfxy.top

find . -mtime -7 -type f
来源：http://drd.guowangkeji.top

[R45] 批量删除
来源：http://ltc.hfpthk.cn

find . -name "*.tmp" -delete
来源：http://nkn.iojbl.cn

[R46] 递归替换文件内容
来源：http://kat.hnxiangtu.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://udt.zycfv.cn

[R47] sed 单行替换
来源：http://nek.jyoumei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://fqb.andypj.xyz

[R48] awk 取指定列
来源：http://utk.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://web.cqqwz.cn

[R49] awk 带条件
来源：http://dgo.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wpf.yj202588.top

[R50] awk 求和
来源：http://gxc.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://nit.kuanghao11.cn

[R51] 排序去重取前几
来源：http://uet.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://xjb.xuetiantiany.cn

[R52] 统计行数
来源：http://fti.feifeiyinyue.top

wc -l a.txt
来源：http://zda.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://yom.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uxr.xylfe.cn

[R54] 比较两个文件
来源：http://hpx.ctjpmb.com

diff a.txt b.txt
来源：http://rff.hongshengwenyu.top

[R55] 压缩与解压
来源：http://sym.jqgufenzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://klg.vehdjk.com

[R56] 远程拷贝
来源：http://doz.iojbl.cn

scp file user@host:/path/
来源：http://xij.0kj1m.cn

[R57] 远程执行命令
来源：http://zsr.dashuyun.cn

ssh user@host 'uptime'
来源：http://uhi.hesvh.cn

[R58] 下载文件
来源：http://obs.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cgs.zdqjudy.top

[R59] 发 POST JSON
来源：http://bfq.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nxg.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://gua.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://way.ybcxt.top

[R61] 磁盘占用
来源：http://tfw.yangfankeji.com

df -h;  du -sh *
来源：http://heb.yongpay.top

[R62] 找最占空间的文件
来源：http://dih.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://ucs.zdbjq.cn

[R63] 内存与进程
来源：http://llb.zhiwuduotai.top

free -h;  ps aux | grep nginx
来源：http://lcp.yuanzhike.top

[R64] 结束进程
来源：http://veg.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://bij.nanxuanxn.top

[R65] 查看端口占用
来源：http://les.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sjq.hysaishi.cn

[R66] 定时任务
来源：http://ddw.guowangkeji.top

crontab -e;  crontab -l
来源：http://nnm.yuxming.cn

[R67] 生成随机十六进制串
来源：http://pld.fzhhl.top

openssl rand -hex 16
来源：http://nsd.yangfankeji.com

[R68] 计算文件校验值
来源：http://zhi.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://obt.zhiwuduotai.top

[R69] 生成随机密码
来源：http://cnh.wangdashe.top

head -c 16 /dev/urandom | base64
来源：http://nwp.nanxinkj.top

[R70] 时间戳与互转
来源：http://zux.cashguo.top

date +%s;  date -d @1700000000
来源：http://erd.cheryme.top

[R71] 日期格式化
来源：http://nsv.snrcjt.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://swj.xinyue.icu

[R72] 等待端口就绪
来源：http://wst.xylfe.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mcw.zhixingplan.top

[R73] 分割大日志
来源：http://bhu.yongpay.top

split -l 1000 big.log part_
来源：http://eds.yj20258.top

[R74] 批量重命名
来源：http://qhx.tian-w.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yzw.gaohongyu789.top

[R75] 导出环境变量
来源：http://ymd.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://oiy.pycfn.com

[R76] 使用临时文件
来源：http://fyd.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ngi.tian-w.cn

[R77] 读取用户输入
来源：http://geg.zhongyouzk.top

read -rp "请输入: " ans
来源：http://yql.yongpay.top

[R78] 交互式菜单
来源：http://hff.yangfankeji.com

select opt in a b c; do echo "$opt"; break; done
来源：http://uqp.pengpengdd.cyou

[R79] 解析命令行选项
来源：http://cvu.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://iag.shuidangran.top

[R80] 查看脚本执行耗时
来源：http://tla.fehbvm.com

time ./run.sh
来源：http://pos.fktsv.cn

================================================================================
来源：http://sld.pycfn.com

S. C / C++ 专题
来源：http://jgv.zdqjudy.top

================================================================================
来源：http://xng.ydzc1.top

[S01] C：Hello World
来源：http://cqo.chenjidiqi.icu

#include <stdio.h>
来源：http://ikm.sweek.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fet.xylfe.cn

[S02] C：变量与格式化输出
来源：http://epu.daria6918.cn

int a = 10; printf("%d\n", a);
来源：http://jlf.zhijiandao.cn

[S03] C：读入整数
来源：http://gik.hnqzz.top

int x; scanf("%d", &x);
来源：http://mca.wangdashe.top

[S04] C：字符串复制
来源：http://xrq.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vix.hnxiangtu.top

[S05] C：字符串长度
来源：http://cxd.ehwqpu.com


<!-- 参考信息 -->