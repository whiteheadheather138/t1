代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://hmb.nanxinkj.top

JOIN users u ON u.id = o.user_id
来源：http://rvp.bjfxy.top

JOIN products p ON p.id = o.product_id;
来源：http://ldq.fanxiaobao.xyz

[Q42] 连接条件附加过滤
来源：http://feq.jinqigfzy.top

SELECT u.name, o.amount FROM users u
来源：http://oil.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://twm.gogol.net.cn

[Q43] 标量子查询
来源：http://kqc.hongshengwenyu.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xet.ydjk.org.cn

[Q44] IN 子查询
来源：http://ozz.pycfn.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://poj.c1oappe.top

[Q45] EXISTS 判断存在
来源：http://edf.jianghu66.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ohm.hcnkem.com

[Q46] NOT EXISTS 判断不存在
来源：http://txg.zhijiandao.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://quq.cqqwz.cn

[Q47] 与平均值比较
来源：http://nfs.daxiang520.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xrm.gotoacloud.top

[Q48] CTE 公用表表达式
来源：http://yil.xingfuxueyuan.xyz

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://nsu.316326.xyz

SELECT * FROM t WHERE c > 5;
来源：http://ugc.ybcxt.top

[Q49] 更新单行
来源：http://dkp.9152youxi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://cpf.cqqwz.cn

[Q50] 批量更新
来源：http://ujc.jyoumei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://uju.tianlin.xyz

[Q51] 用子查询更新
来源：http://rmc.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jrb.zhengqikj.top

[Q52] 删除指定行
来源：http://orh.gaohongyu789.top

DELETE FROM users WHERE id = 10;
来源：http://kcd.zhengqikj.top

[Q53] 按条件删除
来源：http://nns.haohaochexian.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bba.bbcook.cn

[Q54] 清空表
来源：http://ahe.shangyingyoupin.top

TRUNCATE TABLE logs;
来源：http://mjo.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://rjq.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ylm.9152youxi.cn

[Q56] 密集排名（并列不占位）
来源：http://jve.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://idh.chenlongwang.top

[Q57] 行号
来源：http://ved.guannengcc.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dsu.yangfankeji.com

[Q58] 累计求和
来源：http://stg.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wiw.sjlbkw.cn

[Q59] 分组内累计
来源：http://wrn.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aun.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://jbo.shangyingyoupin.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jtc.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jqj.xziqi.cn

[Q61] 移动平均
来源：http://qre.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ahx.yueranfly.top

[Q62] 分组占比
来源：http://wse.cashguo.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jkj.sxryk.cn

[Q63] 开启事务
来源：http://gqk.yuanzhike.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hyt.fengsongda.top

[Q64] 提交事务
来源：http://aqr.chenlongwang.top

COMMIT;
来源：http://vgp.wangdashe.top

[Q65] 回滚事务
来源：http://zpf.vqdsnc.cn

ROLLBACK;
来源：http://ale.0kj1m.cn

[Q66] 行锁查询
来源：http://pao.jinqigufen.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xgq.shanyushiyangtech.top

[Q67] 设置隔离级别
来源：http://wsz.mhx1999.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qhh.zycfv.cn

[Q68] 保存点
来源：http://urg.shanyushiyangkeji.top

SAVEPOINT sp1;
来源：http://bsn.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://xez.shanyushiyangkeji.top

[Q69] 查看执行计划
来源：http://plj.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oet.hnqzz.top

[Q70] 更新统计信息
来源：http://dzl.yj202588.top

ANALYZE TABLE users;
来源：http://wut.yongpay.top

[Q71] 查看建表语句
来源：http://niz.gzhubu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mnn.gaohongyu789.top

[Q72] 查看索引
来源：http://wnw.jinyuanbaomall.cn

SHOW INDEX FROM users;
来源：http://cwc.ehwqpu.com

[Q73] 查看表状态
来源：http://pyv.jinghuilouyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://dpl.gzhubu.top

[Q74] 强制使用索引
来源：http://zan.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kyj.epnwcf.com

[Q75] 日期格式化
来源：http://vrx.jinqigufen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pts.wangdashe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jva.fanxiaobao.xyz

[Q76] 按天统计
来源：http://dwy.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kqx.zhiwuduotai.top

[Q77] 时间加减
来源：http://aic.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://srw.hammf.cn

[Q78] 当前时间
来源：http://euz.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rdr.mhx1999.top

[Q79] 字符串拼接
来源：http://cfp.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ixh.ctjpmb.com

[Q80] 字符串截取
来源：http://pba.zhixingplan.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xzv.gzhubu.top

[Q81] 字符串替换
来源：http://ykr.hongshengwenyu.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gpb.hysaishi.cn

[Q82] 字符长度与字节长度
来源：http://qgf.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eqc.ehwqpu.com

[Q83] 大小写转换
来源：http://fhz.pengpengdd.cyou

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://quh.wangshuangyany.cn

[Q84] 去除首尾空格
来源：http://nfx.jlsjyb.cn

SELECT TRIM(name) FROM users;
来源：http://bmm.pycfn.com

[Q85] 数值取整
来源：http://bif.ywan-chungtsiang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://img.dashuyun.cn

[Q86] 读取 JSON 字段
来源：http://bun.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tdj.jinghuilouyu.cn

[Q87] JSON 字段做条件
来源：http://ysi.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ntg.yueranfly.top

[Q88] 行转列（条件聚合）
来源：http://wfe.sxryk.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ech.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fzm.tian-w.cn

[Q89] 判断表是否存在
来源：http://qjm.sysykeji.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fuf.nwbrower.top

[Q90] 生成序号列
来源：http://pew.hongshengwenyu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://twn.mhx1999.top

================================================================================
来源：http://vkr.andypj.xyz

R. Bash 专题
来源：http://gup.tanke756.top

================================================================================
来源：http://swz.gaohongyu789.top

[R01] shebang 与严格模式
来源：http://jul.yonumen.top

#!/usr/bin/env bash
来源：http://cgo.fanxiaobao.xyz

set -euo pipefail
来源：http://icj.smart0.xyz

[R02] 变量赋值与使用
来源：http://ble.0kj1m.cn

name="Tom"; echo "$name"
来源：http://lxh.jqgufenzy.top

[R03] 只读变量
来源：http://kie.vqdsnc.cn

readonly PI=3.14
来源：http://urx.sweek.top

[R04] 位置参数
来源：http://wrw.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lri.gzhubu.top

[R05] 参数默认值
来源：http://ipm.jinghuilouyu.cn

name="${1:-default}"
来源：http://ryr.tian-w.cn

[R06] 判断命令是否存在
来源：http://hwf.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://phv.ybcxt.top

[R07] if 判断文件
来源：http://cda.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://utw.yangfankeji.com

[R08] 数值比较
来源：http://cdi.fehbvm.com

if (( a > b )); then echo "a 更大"; fi
来源：http://qwv.jqgufenzy.top

[R09] 字符串比较
来源：http://eoz.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dlj.daria6918.cn

[R10] 正则匹配
来源：http://pdq.hcnkem.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrf.zhaomingkeji.xyz

[R11] case 多分支
来源：http://mxx.tarul.cn

case "$1" in
来源：http://aki.daria6918.cn

start) echo "启动" ;;
来源：http://vzz.yj20258.top

stop)  echo "停止" ;;
来源：http://vcn.fzhhl.top

*)     echo "未知命令" ;;
来源：http://vru.yuanzhike.top

esac
来源：http://kpx.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://wrb.vqdsnc.cn

for f in *.txt; do echo "$f"; done
来源：http://kbn.shuidangran.top

[R13] for 计数循环
来源：http://gss.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://ovy.gotoacloud.top

[R14] C 风格 for
来源：http://tkl.pengpengdd.cyou

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tkr.jianghu66.top

[R15] while 逐行读文件
来源：http://vyz.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xxa.wangshuangyany.cn

[R16] until 等待条件
来源：http://nit.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uvh.iojbl.cn

[R17] 数组定义与取值
来源：http://gzl.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://tqt.uphjek.com

[R18] 遍历数组
来源：http://trd.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://okt.jinqigufen.top

[R19] 数组长度
来源：http://zkp.316326.xyz

echo "${#arr[@]}"
来源：http://jpw.jqgufenzy.top

[R20] 关联数组（字典）
来源：http://zmt.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fxh.nwbrower.top

[R21] 字符串长度
来源：http://uyz.zhiwuduotai.top

echo "${#s}"
来源：http://ugd.guowangkeji.top

[R22] 截取子串
来源：http://oaf.zhixingplan.top

echo "${s:0:5}"
来源：http://amk.9152youxi.cn

[R23] 字符串替换
来源：http://vfo.hysaishi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vow.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://lzl.zdqjudy.top

echo "${s^^}"; echo "${s,,}"
来源：http://kmz.dianchejie.cn

[R25] 去后缀 / 去前缀
来源：http://bwy.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mqu.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://ddw.jiagoushi.top

now=$(date +%F); echo "$now"
来源：http://ptb.feifeiyinyue.top

[R27] 算术展开
来源：http://jwy.pycfn.com

echo $((1 + 2 * 3))
来源：http://ezb.nanxinkj.top

[R28] 浮点运算
来源：http://jhs.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://ilu.redwolf501.top

[R29] 定义函数
来源：http://sss.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ziy.tarul.cn

[R30] 函数返回状态码
来源：http://lnu.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://ntb.ydjk.org.cn

[R31] 局部变量
来源：http://xfb.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://pqe.sysykeji.top

[R32] 参数个数校验
来源：http://asz.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wko.xuanzx.com

[R33] 捕获错误并提示行号
来源：http://iwf.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yfc.zhiwuduotai.top

[R34] 退出时清理
来源：http://ntf.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://jlj.kuanghao11.cn

[R35] 后台执行并等待
来源：http://ubv.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kfi.bjfxy.top

[R36] 并发执行多个任务
来源：http://rwf.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://naz.yangfankeji.com

[R37] 把输出赋给变量
来源：http://rjc.jianghu66.top

files=$(ls -1)
来源：http://ztj.redwolf501.top

[R38] 管道串联
来源：http://qfs.yfazqb.com

cat a.txt | grep -i error | wc -l
来源：http://zsf.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://qdm.vehdjk.com

cmd > out.log 2>&1
来源：http://psx.sjlbkw.cn

[R40] 追加写日志
来源：http://eig.52xcode.cn

echo "log" >> out.log
来源：http://wwn.xinyue.icu

[R41] 丢弃输出
来源：http://dih.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://auj.fzhhl.top

[R42] 输入重定向
来源：http://owr.redwolf501.top

wc -l < a.txt
来源：http://sbv.meibo888.top

[R43] 按名字查找文件
来源：http://xbx.nwbrower.top

find . -name "*.log" -type f
来源：http://vol.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://jyb.daxiang520.top

find . -mtime -7 -type f
来源：http://itt.pengpengdd.cyou

[R45] 批量删除
来源：http://zrm.fktsv.cn

find . -name "*.tmp" -delete
来源：http://fom.guannengcc.top

[R46] 递归替换文件内容
来源：http://jvv.shangyingyoupin.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rtp.fanxiaobao.xyz

[R47] sed 单行替换
来源：http://jib.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://npx.nanxuanxn.top

[R48] awk 取指定列
来源：http://dfd.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://wck.jlsjyb.cn

[R49] awk 带条件
来源：http://ksr.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wfb.kuanghao11.cn

[R50] awk 求和
来源：http://sgh.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://whp.kuanghao11.cn

[R51] 排序去重取前几
来源：http://guq.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://rax.jinqigfzy.top

[R52] 统计行数
来源：http://diz.cucudq.cn

wc -l a.txt
来源：http://zjm.jianghu66.top

[R53] 查看文件头与实时尾
来源：http://ypm.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ruc.hcnkem.com

[R54] 比较两个文件
来源：http://ujz.chenjidiqi.icu

diff a.txt b.txt
来源：http://pkc.wangshuangyany.cn

[R55] 压缩与解压
来源：http://qyp.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zac.jinqigufen.top

[R56] 远程拷贝
来源：http://izb.zdqjudy.top

scp file user@host:/path/
来源：http://ewt.tanke756.top

[R57] 远程执行命令
来源：http://apc.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://str.iojbl.cn

[R58] 下载文件
来源：http://dou.pengpengdd.cyou

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://shy.jqgufenzy.top

[R59] 发 POST JSON
来源：http://wxh.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fjc.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://fhq.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qft.ctjpmb.com

[R61] 磁盘占用
来源：http://nuz.dianchejie.cn

df -h;  du -sh *
来源：http://zpa.ydjk.org.cn

[R62] 找最占空间的文件
来源：http://dqk.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://fmx.cucudq.cn

[R63] 内存与进程
来源：http://gmc.uphjek.com

free -h;  ps aux | grep nginx
来源：http://yls.nwbrower.top

[R64] 结束进程
来源：http://vrd.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://miy.xinyue.icu

[R65] 查看端口占用
来源：http://pnx.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vju.jyoumei.cn

[R66] 定时任务
来源：http://rjg.aibaodan.cn

crontab -e;  crontab -l
来源：http://fnx.yj202588.top

[R67] 生成随机十六进制串
来源：http://puu.yangfankeji.com

openssl rand -hex 16
来源：http://bnk.c1oappe.top

[R68] 计算文件校验值
来源：http://aiy.jqgufenzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://eqf.wangshuangyany.cn

[R69] 生成随机密码
来源：http://xwd.chenzaomai.com

head -c 16 /dev/urandom | base64
来源：http://frx.jinqigufen.top

[R70] 时间戳与互转
来源：http://trp.cashguo.top

date +%s;  date -d @1700000000
来源：http://dfe.jqgfzy.top

[R71] 日期格式化
来源：http://eny.birdmap.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://weu.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://lok.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hba.xylfe.cn

[R73] 分割大日志
来源：http://ssw.sysykeji.top

split -l 1000 big.log part_
来源：http://xrv.tianlin.xyz

[R74] 批量重命名
来源：http://ppx.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://teo.hesvh.cn

[R75] 导出环境变量
来源：http://gvc.hesvh.cn

export PATH="$HOME/bin:$PATH"
来源：http://qkm.316326.xyz

[R76] 使用临时文件
来源：http://uid.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czr.quarkkingdee.top

[R77] 读取用户输入
来源：http://eop.epnwcf.com

read -rp "请输入: " ans
来源：http://ywt.vqdsnc.cn

[R78] 交互式菜单
来源：http://obs.meibo888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xpf.xziqi.cn

[R79] 解析命令行选项
来源：http://ero.quarkkingdee.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qpp.smart0.xyz

[R80] 查看脚本执行耗时
来源：http://aov.yueranfly.top

time ./run.sh
来源：http://ara.pengpengdd.cyou

================================================================================
来源：http://sqo.hesvh.cn

S. C / C++ 专题
来源：http://yvo.0kj1m.cn

================================================================================
来源：http://hsc.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://nhz.yuxming.cn

#include <stdio.h>
来源：http://hhe.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://anj.cucudq.cn

[S02] C：变量与格式化输出
来源：http://whb.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://sus.hywenlv.cn

[S03] C：读入整数
来源：http://hak.svipenyu.cn

int x; scanf("%d", &x);
来源：http://zvc.hongshengwenyu.top

[S04] C：字符串复制
来源：http://qal.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bbw.hnxiangtu.top

[S05] C：字符串长度
来源：http://amk.jyoumei.cn

strlen(s)
来源：http://qny.hammf.cn

[S06] C：字符串比较
来源：http://gae.sufxvd.cn

strcmp(a, b) == 0
来源：http://laj.mhx1999.top

[S07] C：数组遍历求和
来源：http://tzf.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cyp.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://brq.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fuj.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://izs.daria6918.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wfh.ydjk.org.cn

[S10] C：指针与解引用
来源：http://yft.52xcode.cn

int *p = &a;  *p = 5;
来源：http://hsn.dianchejie.cn

[S11] C：逐行读文件
来源：http://phm.fehbvm.com


<!-- 参考信息 -->