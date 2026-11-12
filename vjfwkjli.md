代发 wailian999

[Q36] 左连接
来源：http://lnb.feifeiyinyue.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mjg.dashuyun.cn

[Q37] 右连接
来源：http://ovf.iojbl.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://rcr.xuanzx.com

[Q38] 全外连接（PostgreSQL）
来源：http://ute.mhx1999.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://uac.zhijiandao.cn

[Q39] 自连接（查上下级）
来源：http://jro.aibaodan.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://lct.hfpthk.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lyr.zhengqikj.top

[Q40] 交叉连接（笛卡尔积）
来源：http://efr.tianlin.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://dar.fehbvm.com

[Q41] 多表连接
来源：http://yly.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://cau.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://zov.0kj1m.cn

JOIN products p ON p.id = o.product_id;
来源：http://bac.cashguo.top

[Q42] 连接条件附加过滤
来源：http://dby.zhixingplan.top

SELECT u.name, o.amount FROM users u
来源：http://izk.tian-w.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://unp.yangfankeji.com

[Q43] 标量子查询
来源：http://jbu.gotoacloud.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://gmm.snrcjt.cn

[Q44] IN 子查询
来源：http://xxl.fzhhl.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yma.zycfv.cn

[Q45] EXISTS 判断存在
来源：http://xdc.zhongyouzk.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fmz.hnxiangtu.top

[Q46] NOT EXISTS 判断不存在
来源：http://btj.guowangkeji.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://otr.yueranfly.top

[Q47] 与平均值比较
来源：http://nfi.gotoacloud.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://viq.hongshengwenyu.top

[Q48] CTE 公用表表达式
来源：http://vvr.chenzaomai.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qqs.nwbrower.top

SELECT * FROM t WHERE c > 5;
来源：http://kkg.shanyushiyangtech.top

[Q49] 更新单行
来源：http://ipm.nwbrower.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zcj.tanke756.top

[Q50] 批量更新
来源：http://foa.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://drs.gotoacloud.top

[Q51] 用子查询更新
来源：http://cxn.hongshengwenyu.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pih.52xcode.cn

[Q52] 删除指定行
来源：http://opa.yonumen.top

DELETE FROM users WHERE id = 10;
来源：http://avp.guannengcc.top

[Q53] 按条件删除
来源：http://qks.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dcf.epnwcf.com

[Q54] 清空表
来源：http://swt.ywan-chungtsiang.top

TRUNCATE TABLE logs;
来源：http://bkr.havefunace.top

[Q55] 排名（并列占位）
来源：http://mse.jlsjyb.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tkw.yueranfly.top

[Q56] 密集排名（并列不占位）
来源：http://ffd.jinqigufen.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://zhn.dianchejie.cn

[Q57] 行号
来源：http://mnx.9152youxi.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://oid.mhx1999.top

[Q58] 累计求和
来源：http://etm.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jab.fzhhl.top

[Q59] 分组内累计
来源：http://zuy.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rda.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://yld.xinyue.icu

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uyz.meibo888.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ujw.ybcxt.top

[Q61] 移动平均
来源：http://qlh.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cyp.jqgufenzy.top

[Q62] 分组占比
来源：http://xdv.ctjpmb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wgg.mhx1999.top

[Q63] 开启事务
来源：http://ptr.snrcjt.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gbx.sysykeji.top

[Q64] 提交事务
来源：http://wta.xuetiantiany.cn

COMMIT;
来源：http://cco.zhiwuduotai.top

[Q65] 回滚事务
来源：http://cnx.fengsongda.top

ROLLBACK;
来源：http://jhi.9152youxi.cn

[Q66] 行锁查询
来源：http://mes.pengpengdd.cyou

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qit.hfpthk.cn

[Q67] 设置隔离级别
来源：http://zsu.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ncb.snrcjt.cn

[Q68] 保存点
来源：http://rzu.kuanghao11.cn

SAVEPOINT sp1;
来源：http://zln.yuanzhike.top

ROLLBACK TO sp1;
来源：http://qdq.pycfn.com

[Q69] 查看执行计划
来源：http://ldd.xuetiantiany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wht.xinyue.icu

[Q70] 更新统计信息
来源：http://rtd.fehbvm.com

ANALYZE TABLE users;
来源：http://yka.xylfe.cn

[Q71] 查看建表语句
来源：http://nov.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mby.tian-w.cn

[Q72] 查看索引
来源：http://cgc.sweek.top

SHOW INDEX FROM users;
来源：http://gfp.xziqi.cn

[Q73] 查看表状态
来源：http://oyp.hfpthk.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lfw.zdbjq.cn

[Q74] 强制使用索引
来源：http://phd.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fub.fengsongda.top

[Q75] 日期格式化
来源：http://mwh.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jei.tanke756.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qkd.feifeiyinyue.top

[Q76] 按天统计
来源：http://rsv.hnxiangtu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://qwz.yuxming.cn

[Q77] 时间加减
来源：http://edf.jiagoushi.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oqi.yvedp.cn

[Q78] 当前时间
来源：http://she.dashuyun.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://aqh.nwbrower.top

[Q79] 字符串拼接
来源：http://cnd.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rpf.redwolf501.top

[Q80] 字符串截取
来源：http://ysg.snrcjt.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ado.cashguo.top

[Q81] 字符串替换
来源：http://wje.guannengcc.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xor.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://egz.yj202588.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mjt.birdmap.top

[Q83] 大小写转换
来源：http://rfr.sxryk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rdy.ppjwa.cn

[Q84] 去除首尾空格
来源：http://frk.yj20258.top

SELECT TRIM(name) FROM users;
来源：http://jlo.aizwys.cn

[Q85] 数值取整
来源：http://bxz.ydjk.org.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hyq.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://uuz.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gwn.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://mil.fanxiaobao.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jmb.ppjwa.cn

[Q88] 行转列（条件聚合）
来源：http://vfx.ywan-chungtsiang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qae.ppjwa.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tbu.ivvv.top

[Q89] 判断表是否存在
来源：http://npi.guowangkeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fjw.chenlongwang.top

[Q90] 生成序号列
来源：http://vhb.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dkr.cdnleiting.top

================================================================================
来源：http://qkp.hnxiangtu.top

R. Bash 专题
来源：http://dfi.shangyingyoupin.top

================================================================================
来源：http://abx.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://hnu.guowangkeji.top

#!/usr/bin/env bash
来源：http://iwf.zhixingplan.top

set -euo pipefail
来源：http://mwa.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://nrr.c1oappe.top

name="Tom"; echo "$name"
来源：http://ane.meibo888.top

[R03] 只读变量
来源：http://lkj.nanxuanxn.top

readonly PI=3.14
来源：http://sfc.cheryme.top

[R04] 位置参数
来源：http://puq.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tzb.hfpthk.cn

[R05] 参数默认值
来源：http://oir.cucudq.cn

name="${1:-default}"
来源：http://box.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://iga.jlsjyb.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://biq.yj20258888.top

[R07] if 判断文件
来源：http://jnn.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pmy.mhx1999.top

[R08] 数值比较
来源：http://xoo.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bic.hnqzz.top

[R09] 字符串比较
来源：http://tbr.bjfxy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xyh.iojbl.cn

[R10] 正则匹配
来源：http://cfo.cqqwz.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dez.316326.xyz

[R11] case 多分支
来源：http://aqk.yueranfly.top

case "$1" in
来源：http://ick.ehwqpu.com

start) echo "启动" ;;
来源：http://pnn.jinqigfzy.top

stop)  echo "停止" ;;
来源：http://xtf.smart0.xyz

*)     echo "未知命令" ;;
来源：http://nth.tianlin.xyz

esac
来源：http://fup.feifeiyinyue.top

[R12] for 遍历文件
来源：http://mha.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://sjm.havefunace.top

[R13] for 计数循环
来源：http://lor.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://mtf.jlsjyb.cn

[R14] C 风格 for
来源：http://rsz.nwbrower.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://oug.cucudq.cn

[R15] while 逐行读文件
来源：http://rey.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dts.daxiang520.top

[R16] until 等待条件
来源：http://vhp.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ehx.snrcjt.cn

[R17] 数组定义与取值
来源：http://vzn.xziqi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://lha.shuidangran.top

[R18] 遍历数组
来源：http://lpp.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qwu.fanxiaobao.xyz

[R19] 数组长度
来源：http://isq.wangdashe.top

echo "${#arr[@]}"
来源：http://jgx.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://pme.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aou.yuxming.cn

[R21] 字符串长度
来源：http://ovq.bjfxy.top

echo "${#s}"
来源：http://xbd.zhengqikj.top

[R22] 截取子串
来源：http://kje.meibo888.top

echo "${s:0:5}"
来源：http://wyl.pycfn.com

[R23] 字符串替换
来源：http://mzz.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gzi.wangdashe.top

[R24] 大小写转换
来源：http://oky.svipenyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rlz.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://cgj.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wwi.redwolf501.top

[R26] 命令替换
来源：http://qyd.yonumen.top

now=$(date +%F); echo "$now"
来源：http://vjm.jinyuanbaomall.cn

[R27] 算术展开
来源：http://jpq.fzhhl.top

echo $((1 + 2 * 3))
来源：http://rgj.hongshengwenyu.top

[R28] 浮点运算
来源：http://obi.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://nly.zhiwuduotai.top

[R29] 定义函数
来源：http://naa.ctjpmb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dvo.jqgufenzy.top

[R30] 函数返回状态码
来源：http://esg.52xcode.cn

f() { return 0; }; f || echo "失败了"
来源：http://vhe.daria6918.cn

[R31] 局部变量
来源：http://hga.ppjwa.cn

f() { local x=1; echo "$x"; }
来源：http://tyq.xuetiantiany.cn

[R32] 参数个数校验
来源：http://zcf.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zzo.chenzaomai.com

[R33] 捕获错误并提示行号
来源：http://ozx.nanxinkj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uru.gogol.net.cn

[R34] 退出时清理
来源：http://yhx.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://pem.zycfv.cn

[R35] 后台执行并等待
来源：http://gfc.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://het.gotoacloud.top

[R36] 并发执行多个任务
来源：http://sqs.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eni.jiagoushi.top

[R37] 把输出赋给变量
来源：http://lmd.yfazqb.com

files=$(ls -1)
来源：http://ffh.vqdsnc.cn

[R38] 管道串联
来源：http://zvo.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://yln.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://gmv.dashuyun.cn

cmd > out.log 2>&1
来源：http://xix.iojbl.cn

[R40] 追加写日志
来源：http://lcz.andypj.xyz

echo "log" >> out.log
来源：http://hih.iojbl.cn

[R41] 丢弃输出
来源：http://olz.fehbvm.com

cmd >/dev/null 2>&1
来源：http://wmq.epnwcf.com

[R42] 输入重定向
来源：http://qzy.hcnkem.com

wc -l < a.txt
来源：http://qdy.gzhubu.top

[R43] 按名字查找文件
来源：http://eaw.hnqzz.top

find . -name "*.log" -type f
来源：http://clh.chenlongwang.top

[R44] 按修改时间查找
来源：http://jld.jqgufenzy.top

find . -mtime -7 -type f
来源：http://soe.ppjwa.cn

[R45] 批量删除
来源：http://tcl.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://qio.hfpthk.cn

[R46] 递归替换文件内容
来源：http://yps.316326.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bzk.zhengqikj.top

[R47] sed 单行替换
来源：http://ytt.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://tcq.xinyue.icu

[R48] awk 取指定列
来源：http://brp.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://uip.daria6918.cn

[R49] awk 带条件
来源：http://wzt.cheryme.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rci.zhijiandao.cn

[R50] awk 求和
来源：http://weh.tianlin.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://xgx.quarkkingdee.top

[R51] 排序去重取前几
来源：http://hws.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fns.xinyue.icu

[R52] 统计行数
来源：http://ovw.jinqigfzy.top

wc -l a.txt
来源：http://ulr.zhiwuduotai.top

[R53] 查看文件头与实时尾
来源：http://fgt.xuetiantiany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mpd.9152youxi.cn

[R54] 比较两个文件
来源：http://ehp.tian-w.cn

diff a.txt b.txt
来源：http://zck.cdnleiting.top

[R55] 压缩与解压
来源：http://dan.shzxlz.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://olr.zhixingplan.top

[R56] 远程拷贝
来源：http://nmg.pengpengdd.cyou

scp file user@host:/path/
来源：http://tcw.hongshengwenyu.top

[R57] 远程执行命令
来源：http://uwn.nanxinkj.top

ssh user@host 'uptime'
来源：http://dji.ctjpmb.com

[R58] 下载文件
来源：http://hji.sysykeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zpj.bjfxy.top

[R59] 发 POST JSON
来源：http://vgs.yj20258888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vac.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://myh.hfpthk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ekr.yuxming.cn

[R61] 磁盘占用
来源：http://pmp.cdnleiting.top

df -h;  du -sh *
来源：http://fjg.fanxiaobao.xyz

[R62] 找最占空间的文件
来源：http://csa.svipenyu.cn

du -ah . | sort -rh | head -10
来源：http://lep.dashuyun.cn

[R63] 内存与进程
来源：http://uww.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://oyy.hfpthk.cn

[R64] 结束进程
来源：http://uyd.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://zgf.wangshuangyany.cn

[R65] 查看端口占用
来源：http://xck.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://syr.c1oappe.top

[R66] 定时任务
来源：http://ajr.gzhubu.top

crontab -e;  crontab -l
来源：http://pta.daxiang520.top

[R67] 生成随机十六进制串
来源：http://eaq.shanyushiyangtech.top

openssl rand -hex 16
来源：http://qxp.fengsongda.top

[R68] 计算文件校验值
来源：http://qog.guowangkeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://pbn.jinyuanbaomall.cn

[R69] 生成随机密码
来源：http://njg.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://rug.guowangkeji.top

[R70] 时间戳与互转
来源：http://dth.hammf.cn

date +%s;  date -d @1700000000
来源：http://cxo.aibaodan.cn

[R71] 日期格式化
来源：http://aom.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xof.jinqigufen.top

[R72] 等待端口就绪
来源：http://ezr.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ocm.nanxinkj.top

[R73] 分割大日志
来源：http://uch.yj20258.top

split -l 1000 big.log part_
来源：http://nvb.zdbjq.cn

[R74] 批量重命名
来源：http://gtm.jinghuilouyu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://woq.yonumen.top

[R75] 导出环境变量
来源：http://gch.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://mbm.hcnkem.com

[R76] 使用临时文件
来源：http://xvg.nanxuanxn.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wjp.yanxiufei.cn

[R77] 读取用户输入
来源：http://itb.hammf.cn

read -rp "请输入: " ans
来源：http://ycj.hesvh.cn

[R78] 交互式菜单
来源：http://myt.daxiang520.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ruz.guannengcc.top

[R79] 解析命令行选项
来源：http://nvx.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fwf.sufxvd.cn

[R80] 查看脚本执行耗时
来源：http://ddo.hcnkem.com

time ./run.sh
来源：http://qkr.yueranfly.top

================================================================================
来源：http://drc.yvedp.cn

S. C / C++ 专题
来源：http://fpe.fengsongda.top

================================================================================
来源：http://mmr.sjlbkw.cn

[S01] C：Hello World
来源：http://boi.nwbrower.top

#include <stdio.h>
来源：http://oyn.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yrn.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://vqt.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://asa.jlsjyb.cn

[S03] C：读入整数
来源：http://adu.sxryk.cn

int x; scanf("%d", &x);
来源：http://upo.redwolf501.top

[S04] C：字符串复制
来源：http://kre.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://hzs.9152youxi.cn

[S05] C：字符串长度
来源：http://hxu.9152youxi.cn


<!-- 参考信息 -->