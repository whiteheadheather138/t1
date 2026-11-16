代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://dyx.zdbjq.cn

JOIN users u ON u.id = o.user_id
来源：http://cqg.shzxlz.cn

JOIN products p ON p.id = o.product_id;
来源：http://cqg.svipenyu.cn

[Q42] 连接条件附加过滤
来源：http://etj.tian-w.cn

SELECT u.name, o.amount FROM users u
来源：http://srp.cdnleiting.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://cip.jinqigfzy.top

[Q43] 标量子查询
来源：http://ngb.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://nti.zhengqikj.top

[Q44] IN 子查询
来源：http://xou.yongpay.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zcf.ydjk.org.cn

[Q45] EXISTS 判断存在
来源：http://ptw.zhoulong.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jbi.cashguo.top

[Q46] NOT EXISTS 判断不存在
来源：http://obo.pengpengdd.cyou

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xtn.yangfankeji.com

[Q47] 与平均值比较
来源：http://itl.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fyo.ydzc1.top

[Q48] CTE 公用表表达式
来源：http://ebi.cheryme.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ujg.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://gha.wangdashe.top

[Q49] 更新单行
来源：http://bda.daria6918.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ndl.xuetiantiany.cn

[Q50] 批量更新
来源：http://gkh.nwbrower.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zns.mhx1999.top

[Q51] 用子查询更新
来源：http://xiq.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xix.sysykeji.top

[Q52] 删除指定行
来源：http://oiz.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://jpb.yueranfly.top

[Q53] 按条件删除
来源：http://gmb.dashuyun.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://tuz.chenzaomai.com

[Q54] 清空表
来源：http://fgy.jqgfzy.top

TRUNCATE TABLE logs;
来源：http://opk.xuanzx.com

[Q55] 排名（并列占位）
来源：http://evu.pycfn.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fdk.xuetiantiany.cn

[Q56] 密集排名（并列不占位）
来源：http://ggl.gzhubu.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wgq.zdqjudy.top

[Q57] 行号
来源：http://ztd.daxiang520.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gwu.jianghu66.top

[Q58] 累计求和
来源：http://dgt.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://gic.0kj1m.cn

[Q59] 分组内累计
来源：http://jdi.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://don.hcnkem.com

[Q60] 取上一行 / 下一行
来源：http://mzi.zdqjudy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://utm.yvedp.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eio.fanxiaobao.xyz

[Q61] 移动平均
来源：http://qik.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xox.daxiang520.top

[Q62] 分组占比
来源：http://dig.nwbrower.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kpe.jinqigufen.top

[Q63] 开启事务
来源：http://jyg.epnwcf.com

START TRANSACTION;                -- 或 BEGIN
来源：http://tbs.fktsv.cn

[Q64] 提交事务
来源：http://aew.fehbvm.com

COMMIT;
来源：http://lrn.c1oappe.top

[Q65] 回滚事务
来源：http://len.hfpthk.cn

ROLLBACK;
来源：http://exg.52xcode.cn

[Q66] 行锁查询
来源：http://law.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xnw.tianlin.xyz

[Q67] 设置隔离级别
来源：http://qne.zhijiandao.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fcu.jqgfzy.top

[Q68] 保存点
来源：http://guz.smart0.xyz

SAVEPOINT sp1;
来源：http://six.xuanzx.com

ROLLBACK TO sp1;
来源：http://iqp.vqdsnc.cn

[Q69] 查看执行计划
来源：http://qpm.tanke756.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zcc.vqdsnc.cn

[Q70] 更新统计信息
来源：http://jkl.ybcxt.top

ANALYZE TABLE users;
来源：http://sxj.guowangkeji.top

[Q71] 查看建表语句
来源：http://bag.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jbc.shangyingyoupin.top

[Q72] 查看索引
来源：http://rke.jinghuilouyu.cn

SHOW INDEX FROM users;
来源：http://yoa.andypj.xyz

[Q73] 查看表状态
来源：http://lah.hnxiangtu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://frh.hcnkem.com

[Q74] 强制使用索引
来源：http://naz.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://opn.tarul.cn

[Q75] 日期格式化
来源：http://kie.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qxo.zhengqikj.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yuw.daxiang520.top

[Q76] 按天统计
来源：http://ehm.52xcode.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nal.kuanghao11.cn

[Q77] 时间加减
来源：http://zok.xylfe.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cth.yj202588.top

[Q78] 当前时间
来源：http://veo.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lun.jianghu66.top

[Q79] 字符串拼接
来源：http://mgj.birdmap.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pzz.bbcook.cn

[Q80] 字符串截取
来源：http://xka.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lpd.jqgfzy.top

[Q81] 字符串替换
来源：http://rbe.zhixingplan.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gwa.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://cbp.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zxo.gotoacloud.top

[Q83] 大小写转换
来源：http://sev.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://svr.xziqi.cn

[Q84] 去除首尾空格
来源：http://cyq.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://ilm.hongshengwenyu.top

[Q85] 数值取整
来源：http://ynb.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lja.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://qfj.jianghu66.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ciz.epnwcf.com

[Q87] JSON 字段做条件
来源：http://lkt.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://sos.jinyuanbaomall.cn

[Q88] 行转列（条件聚合）
来源：http://phb.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://srx.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://njp.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://uqj.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mno.cucudq.cn

[Q90] 生成序号列
来源：http://edp.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gbq.yfazqb.com

================================================================================
来源：http://pia.jlsjyb.cn

R. Bash 专题
来源：http://wcb.daxiang520.top

================================================================================
来源：http://nsw.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://akn.yuxming.cn

#!/usr/bin/env bash
来源：http://bws.svipenyu.cn

set -euo pipefail
来源：http://ywv.guannengcc.top

[R02] 变量赋值与使用
来源：http://bae.yuxming.cn

name="Tom"; echo "$name"
来源：http://lol.zdbjq.cn

[R03] 只读变量
来源：http://qyc.nanxuanxn.top

readonly PI=3.14
来源：http://tsl.epnwcf.com

[R04] 位置参数
来源：http://sim.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oee.yuanzhike.top

[R05] 参数默认值
来源：http://pde.xylfe.cn

name="${1:-default}"
来源：http://cjo.nwbrower.top

[R06] 判断命令是否存在
来源：http://vbg.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jpv.dianchejie.cn

[R07] if 判断文件
来源：http://mju.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rug.ppjwa.cn

[R08] 数值比较
来源：http://vsf.kuanghao11.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rvh.zhongyouzk.top

[R09] 字符串比较
来源：http://xbn.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pzk.hnxiangtu.top

[R10] 正则匹配
来源：http://zak.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bwa.yangfankeji.com

[R11] case 多分支
来源：http://ksm.sufxvd.cn

case "$1" in
来源：http://buq.sxryk.cn

start) echo "启动" ;;
来源：http://ogt.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://ubf.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://bkq.yj20258888.top

esac
来源：http://yar.sxryk.cn

[R12] for 遍历文件
来源：http://hjn.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://udu.ydzc1.top

[R13] for 计数循环
来源：http://nwa.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://uuc.kuanghao11.cn

[R14] C 风格 for
来源：http://rex.chenjidiqi.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rcu.redwolf501.top

[R15] while 逐行读文件
来源：http://wcl.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baa.cucudq.cn

[R16] until 等待条件
来源：http://duh.xuetiantiany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bkg.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://xzu.meibo888.top

arr=(a b c); echo "${arr[0]}"
来源：http://gwg.zhongyouzk.top

[R18] 遍历数组
来源：http://oea.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cmu.svipenyu.cn

[R19] 数组长度
来源：http://bip.uphjek.com

echo "${#arr[@]}"
来源：http://czh.zhixingplan.top

[R20] 关联数组（字典）
来源：http://xda.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jrt.316326.xyz

[R21] 字符串长度
来源：http://xsa.jlsjyb.cn

echo "${#s}"
来源：http://qab.zhiwuduotai.top

[R22] 截取子串
来源：http://snq.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://zfr.wangdashe.top

[R23] 字符串替换
来源：http://nis.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hcy.hysaishi.cn

[R24] 大小写转换
来源：http://yew.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://rib.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://sxk.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://myh.bjfxy.top

[R26] 命令替换
来源：http://osl.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://gss.fktsv.cn

[R27] 算术展开
来源：http://lxf.gogol.net.cn

echo $((1 + 2 * 3))
来源：http://tvr.ivvv.top

[R28] 浮点运算
来源：http://tyh.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://tiy.sysykeji.top

[R29] 定义函数
来源：http://okg.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ert.0kj1m.cn

[R30] 函数返回状态码
来源：http://zac.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://fui.bjfxy.top

[R31] 局部变量
来源：http://aya.shanyushiyangtech.top

f() { local x=1; echo "$x"; }
来源：http://bec.zdqjudy.top

[R32] 参数个数校验
来源：http://tvi.cqqwz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fjd.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://qzr.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tmp.sufxvd.cn

[R34] 退出时清理
来源：http://oad.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fvt.iojbl.cn

[R35] 后台执行并等待
来源：http://ctb.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ibc.zhaomingkeji.xyz

[R36] 并发执行多个任务
来源：http://cwr.316326.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kmx.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://vri.bjfxy.top

files=$(ls -1)
来源：http://pxa.hcnkem.com

[R38] 管道串联
来源：http://iup.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://xhh.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://uxo.redwolf501.top

cmd > out.log 2>&1
来源：http://rxl.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://nml.hongshengwenyu.top

echo "log" >> out.log
来源：http://djp.hnqzz.top

[R41] 丢弃输出
来源：http://bnz.birdmap.top

cmd >/dev/null 2>&1
来源：http://kwr.cdnleiting.top

[R42] 输入重定向
来源：http://hoy.gaohongyu789.top

wc -l < a.txt
来源：http://muz.nanxuanxn.top

[R43] 按名字查找文件
来源：http://hoj.sufxvd.cn

find . -name "*.log" -type f
来源：http://vlb.hnqzz.top

[R44] 按修改时间查找
来源：http://oti.dianchejie.cn

find . -mtime -7 -type f
来源：http://lbb.cheryme.top

[R45] 批量删除
来源：http://ecg.zhijiandao.cn

find . -name "*.tmp" -delete
来源：http://iwq.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://aff.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rnj.sweek.top

[R47] sed 单行替换
来源：http://vom.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://wxe.nanxuanxn.top

[R48] awk 取指定列
来源：http://mxi.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://onc.yj20258888.top

[R49] awk 带条件
来源：http://pmn.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ium.gogol.net.cn

[R50] awk 求和
来源：http://dgd.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bpw.hywenlv.cn

[R51] 排序去重取前几
来源：http://rhm.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://peh.gzhubu.top

[R52] 统计行数
来源：http://idn.yonumen.top

wc -l a.txt
来源：http://kvb.uphjek.com

[R53] 查看文件头与实时尾
来源：http://qeq.yj202588.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jqm.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://mis.shuidangran.top

diff a.txt b.txt
来源：http://fmm.sxryk.cn

[R55] 压缩与解压
来源：http://lvw.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gwq.jinghuilouyu.cn

[R56] 远程拷贝
来源：http://wuu.jinqigfzy.top

scp file user@host:/path/
来源：http://etg.yangfankeji.com

[R57] 远程执行命令
来源：http://roy.jinqigfzy.top

ssh user@host 'uptime'
来源：http://par.gaohongyu789.top

[R58] 下载文件
来源：http://ryw.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uga.chenlongwang.top

[R59] 发 POST JSON
来源：http://yrp.shanyushiyangtech.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oun.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://cnd.hnqzz.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://akw.daria6918.cn

[R61] 磁盘占用
来源：http://gim.aibaodan.cn

df -h;  du -sh *
来源：http://ajp.quarkkingdee.top

[R62] 找最占空间的文件
来源：http://pkw.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://ovy.shangyingyoupin.top

[R63] 内存与进程
来源：http://kpv.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://pks.gogol.net.cn

[R64] 结束进程
来源：http://jmv.yangfankeji.com

kill -9 $(pgrep -f app.py)
来源：http://gwc.nanxinkj.top

[R65] 查看端口占用
来源：http://jso.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ryp.uphjek.com

[R66] 定时任务
来源：http://zfy.zhixingplan.top

crontab -e;  crontab -l
来源：http://tem.cdnleiting.top

[R67] 生成随机十六进制串
来源：http://zsw.316326.xyz

openssl rand -hex 16
来源：http://asn.jyoumei.cn

[R68] 计算文件校验值
来源：http://glc.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://car.9152youxi.cn

[R69] 生成随机密码
来源：http://vjj.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://moj.ppjwa.cn

[R70] 时间戳与互转
来源：http://okl.tianlin.xyz

date +%s;  date -d @1700000000
来源：http://kuf.zhengqikj.top

[R71] 日期格式化
来源：http://vdd.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nrq.smart0.xyz

[R72] 等待端口就绪
来源：http://ang.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hrd.uphjek.com

[R73] 分割大日志
来源：http://zil.zhijiandao.cn

split -l 1000 big.log part_
来源：http://qzw.uphjek.com

[R74] 批量重命名
来源：http://tnc.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wdc.xziqi.cn

[R75] 导出环境变量
来源：http://gfe.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://grx.yfazqb.com

[R76] 使用临时文件
来源：http://dvq.havefunace.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bsh.yueranfly.top

[R77] 读取用户输入
来源：http://awi.xylfe.cn

read -rp "请输入: " ans
来源：http://lux.yangfankeji.com

[R78] 交互式菜单
来源：http://kru.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://piq.guannengcc.top

[R79] 解析命令行选项
来源：http://lqx.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://egu.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://wez.zhiwuduotai.top

time ./run.sh
来源：http://jrg.tarul.cn

================================================================================
来源：http://mgj.tian-w.cn

S. C / C++ 专题
来源：http://jzg.tarul.cn

================================================================================
来源：http://ohn.vqdsnc.cn

[S01] C：Hello World
来源：http://pji.hysaishi.cn

#include <stdio.h>
来源：http://ncs.ybcxt.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vme.cucudq.cn

[S02] C：变量与格式化输出
来源：http://ghs.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://aae.bjfxy.top

[S03] C：读入整数
来源：http://dgj.sjlbkw.cn

int x; scanf("%d", &x);
来源：http://hdk.yfazqb.com

[S04] C：字符串复制
来源：http://law.hywenlv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ehi.hfpthk.cn

[S05] C：字符串长度
来源：http://jtr.pycfn.com

strlen(s)
来源：http://dat.shzxlz.cn

[S06] C：字符串比较
来源：http://zin.ybcxt.top

strcmp(a, b) == 0
来源：http://ucg.dianchejie.cn

[S07] C：数组遍历求和
来源：http://vry.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rbm.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://igg.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lor.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://vhu.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://okc.hysaishi.cn

[S10] C：指针与解引用
来源：http://uuh.0kj1m.cn

int *p = &a;  *p = 5;
来源：http://kfq.wangdashe.top

[S11] C：逐行读文件
来源：http://uze.jyoumei.cn


<!-- 参考信息 -->