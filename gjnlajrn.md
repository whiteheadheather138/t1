代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://exm.zdqjudy.top

JOIN users u ON u.id = o.user_id
来源：http://bqf.tarul.cn

JOIN products p ON p.id = o.product_id;
来源：http://jyl.xuanzx.com

[Q42] 连接条件附加过滤
来源：http://xou.yonumen.top

SELECT u.name, o.amount FROM users u
来源：http://qez.shangyingyoupin.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://twx.zhixingplan.top

[Q43] 标量子查询
来源：http://ndj.guannengcc.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eom.cashguo.top

[Q44] IN 子查询
来源：http://qfw.zdqjudy.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zoc.hnxiangtu.top

[Q45] EXISTS 判断存在
来源：http://ifr.fanxiaobao.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hzr.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://qng.yonumen.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zuc.sysykeji.top

[Q47] 与平均值比较
来源：http://vcq.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wcb.shuidangran.top

[Q48] CTE 公用表表达式
来源：http://vyi.vehdjk.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tts.andypj.xyz

SELECT * FROM t WHERE c > 5;
来源：http://hem.zhengqikj.top

[Q49] 更新单行
来源：http://okp.tarul.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://boo.hysaishi.cn

[Q50] 批量更新
来源：http://rix.yuxming.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pdd.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://qcs.hammf.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zlz.nanxinkj.top

[Q52] 删除指定行
来源：http://kje.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://amb.mhx1999.top

[Q53] 按条件删除
来源：http://omr.sjlbkw.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pub.shangyingyoupin.top

[Q54] 清空表
来源：http://bip.cashguo.top

TRUNCATE TABLE logs;
来源：http://woh.ydjk.org.cn

[Q55] 排名（并列占位）
来源：http://xqr.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ral.ydzc1.top

[Q56] 密集排名（并列不占位）
来源：http://ccw.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hpd.ybcxt.top

[Q57] 行号
来源：http://ncg.hesvh.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://abd.jiagoushi.top

[Q58] 累计求和
来源：http://bfw.sufxvd.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://can.chenjidiqi.icu

[Q59] 分组内累计
来源：http://wtv.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kuo.xylfe.cn

[Q60] 取上一行 / 下一行
来源：http://vks.gotoacloud.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zpu.fanxiaobao.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rgu.316326.xyz

[Q61] 移动平均
来源：http://cyn.xuanzx.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vbh.xylfe.cn

[Q62] 分组占比
来源：http://ksp.ydjk.org.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://php.tanke756.top

[Q63] 开启事务
来源：http://hby.zdqjudy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://deo.hnxiangtu.top

[Q64] 提交事务
来源：http://omq.wangshuangyany.cn

COMMIT;
来源：http://ypt.sxryk.cn

[Q65] 回滚事务
来源：http://qmr.zycfv.cn

ROLLBACK;
来源：http://dpn.xinyue.icu

[Q66] 行锁查询
来源：http://cvy.hysaishi.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://uai.kuanghao11.cn

[Q67] 设置隔离级别
来源：http://sfd.yongpay.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pqy.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://hsc.jianghu66.top

SAVEPOINT sp1;
来源：http://cav.aizwys.cn

ROLLBACK TO sp1;
来源：http://znz.cqqwz.cn

[Q69] 查看执行计划
来源：http://xgz.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://omi.xingfuxueyuan.xyz

[Q70] 更新统计信息
来源：http://uwj.gaohongyu789.top

ANALYZE TABLE users;
来源：http://wxj.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://xqq.vqdsnc.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ijb.zhaomingkeji.xyz

[Q72] 查看索引
来源：http://uwc.chenzaomai.com

SHOW INDEX FROM users;
来源：http://sng.yangfankeji.com

[Q73] 查看表状态
来源：http://fjq.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yqe.gogol.net.cn

[Q74] 强制使用索引
来源：http://pan.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tlv.gzhubu.top

[Q75] 日期格式化
来源：http://cmq.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wtk.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fxt.havefunace.top

[Q76] 按天统计
来源：http://ube.0kj1m.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ujr.vqdsnc.cn

[Q77] 时间加减
来源：http://pqz.zhoulong.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://abw.pengpengdd.cyou

[Q78] 当前时间
来源：http://bdf.nanxinkj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rzo.snrcjt.cn

[Q79] 字符串拼接
来源：http://lpq.xuanzx.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gui.jinqigfzy.top

[Q80] 字符串截取
来源：http://glx.xziqi.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wud.dianchejie.cn

[Q81] 字符串替换
来源：http://sav.jianghu66.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jrf.shanyushiyangtech.top

[Q82] 字符长度与字节长度
来源：http://rak.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://anf.zycfv.cn

[Q83] 大小写转换
来源：http://nyv.birdmap.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://guw.redwolf501.top

[Q84] 去除首尾空格
来源：http://kpa.nwbrower.top

SELECT TRIM(name) FROM users;
来源：http://uab.yueranfly.top

[Q85] 数值取整
来源：http://duc.chenlongwang.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://pbp.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://vha.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vbo.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://ido.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pwn.cdnleiting.top

[Q88] 行转列（条件聚合）
来源：http://ele.shangyingyoupin.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vrq.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://met.sjlbkw.cn

[Q89] 判断表是否存在
来源：http://vaj.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ghq.sysykeji.top

[Q90] 生成序号列
来源：http://dbm.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vij.gogol.net.cn

================================================================================
来源：http://efu.ydjk.org.cn

R. Bash 专题
来源：http://fov.sysykeji.top

================================================================================
来源：http://vcn.sufxvd.cn

[R01] shebang 与严格模式
来源：http://hmz.quarkkingdee.top

#!/usr/bin/env bash
来源：http://vao.bjfxy.top

set -euo pipefail
来源：http://pdq.zhengqikj.top

[R02] 变量赋值与使用
来源：http://nzh.xuanzx.com

name="Tom"; echo "$name"
来源：http://lry.c1oappe.top

[R03] 只读变量
来源：http://esi.fanxiaobao.xyz

readonly PI=3.14
来源：http://ame.fanxiaobao.xyz

[R04] 位置参数
来源：http://oyg.yj20258.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://apc.jqgufenzy.top

[R05] 参数默认值
来源：http://wni.birdmap.top

name="${1:-default}"
来源：http://eky.redwolf501.top

[R06] 判断命令是否存在
来源：http://bwq.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sgp.yanxiufei.cn

[R07] if 判断文件
来源：http://rwe.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zhz.cheryme.top

[R08] 数值比较
来源：http://jwv.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbz.bjfxy.top

[R09] 字符串比较
来源：http://ltq.hammf.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tpd.zdqjudy.top

[R10] 正则匹配
来源：http://amb.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nyw.sxryk.cn

[R11] case 多分支
来源：http://abp.guowangkeji.top

case "$1" in
来源：http://skr.ywan-chungtsiang.top

start) echo "启动" ;;
来源：http://lso.feifeiyinyue.top

stop)  echo "停止" ;;
来源：http://lhh.ehwqpu.com

*)     echo "未知命令" ;;
来源：http://mlb.jinqigufen.top

esac
来源：http://mdq.zhixingplan.top

[R12] for 遍历文件
来源：http://aze.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://dtp.cashguo.top

[R13] for 计数循环
来源：http://obr.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://sin.epnwcf.com

[R14] C 风格 for
来源：http://ecm.ydzc1.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iho.smart0.xyz

[R15] while 逐行读文件
来源：http://qbp.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mgf.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://umq.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hxj.cheryme.top

[R17] 数组定义与取值
来源：http://zcs.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://kxz.tianlin.xyz

[R18] 遍历数组
来源：http://qga.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vse.cqqwz.cn

[R19] 数组长度
来源：http://jlr.cucudq.cn

echo "${#arr[@]}"
来源：http://ooc.ppjwa.cn

[R20] 关联数组（字典）
来源：http://xuk.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ddj.hesvh.cn

[R21] 字符串长度
来源：http://ggm.wangshuangyany.cn

echo "${#s}"
来源：http://tsn.kuanghao11.cn

[R22] 截取子串
来源：http://wwf.xinyue.icu

echo "${s:0:5}"
来源：http://mcq.zhengqikj.top

[R23] 字符串替换
来源：http://usg.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gqd.yj20258888.top

[R24] 大小写转换
来源：http://kpw.hcnkem.com

echo "${s^^}"; echo "${s,,}"
来源：http://tfb.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://bzk.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://rar.cqqwz.cn

[R26] 命令替换
来源：http://lcr.xuetiantiany.cn

now=$(date +%F); echo "$now"
来源：http://rem.hysaishi.cn

[R27] 算术展开
来源：http://ftz.cucudq.cn

echo $((1 + 2 * 3))
来源：http://awk.hammf.cn

[R28] 浮点运算
来源：http://zbm.yuanzhike.top

echo "scale=2; 10/3" | bc
来源：http://uun.feifeiyinyue.top

[R29] 定义函数
来源：http://nnh.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mgs.ppjwa.cn

[R30] 函数返回状态码
来源：http://uaj.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://hvr.fanxiaobao.xyz

[R31] 局部变量
来源：http://mbm.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://whr.hywenlv.cn

[R32] 参数个数校验
来源：http://ygu.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://slj.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://wpp.shangyingyoupin.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vof.hfpthk.cn

[R34] 退出时清理
来源：http://non.gzhubu.top

trap 'rm -f "$tmp"' EXIT
来源：http://pml.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://myn.52xcode.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://owi.jianghu66.top

[R36] 并发执行多个任务
来源：http://wrm.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://upd.cqqwz.cn

[R37] 把输出赋给变量
来源：http://gnl.pycfn.com

files=$(ls -1)
来源：http://lzr.sufxvd.cn

[R38] 管道串联
来源：http://aov.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://jhl.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://ooc.yfazqb.com

cmd > out.log 2>&1
来源：http://atp.9152youxi.cn

[R40] 追加写日志
来源：http://rdj.hesvh.cn

echo "log" >> out.log
来源：http://mtf.bjfxy.top

[R41] 丢弃输出
来源：http://kbm.xuanzx.com

cmd >/dev/null 2>&1
来源：http://zxn.ctjpmb.com

[R42] 输入重定向
来源：http://mkl.daria6918.cn

wc -l < a.txt
来源：http://fmk.aizwys.cn

[R43] 按名字查找文件
来源：http://mmt.yueranfly.top

find . -name "*.log" -type f
来源：http://fag.gzhubu.top

[R44] 按修改时间查找
来源：http://ukb.cdnleiting.top

find . -mtime -7 -type f
来源：http://jyq.svipenyu.cn

[R45] 批量删除
来源：http://xpv.yanxiufei.cn

find . -name "*.tmp" -delete
来源：http://hmp.zdqjudy.top

[R46] 递归替换文件内容
来源：http://nlp.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gaj.hesvh.cn

[R47] sed 单行替换
来源：http://esv.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://wcb.pengpengdd.cyou

[R48] awk 取指定列
来源：http://izf.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://wxx.iojbl.cn

[R49] awk 带条件
来源：http://gdw.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qqx.gogol.net.cn

[R50] awk 求和
来源：http://mut.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://uvr.yangfankeji.com

[R51] 排序去重取前几
来源：http://trn.chenjidiqi.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://qre.yuanzhike.top

[R52] 统计行数
来源：http://wbz.quarkkingdee.top

wc -l a.txt
来源：http://wiy.hammf.cn

[R53] 查看文件头与实时尾
来源：http://dcd.ydjk.org.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wyn.9152youxi.cn

[R54] 比较两个文件
来源：http://iey.zhoulong.xyz

diff a.txt b.txt
来源：http://rtb.yuanzhike.top

[R55] 压缩与解压
来源：http://gtq.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ctj.sxryk.cn

[R56] 远程拷贝
来源：http://pzy.c1oappe.top

scp file user@host:/path/
来源：http://rzo.gzhubu.top

[R57] 远程执行命令
来源：http://lpj.hywenlv.cn

ssh user@host 'uptime'
来源：http://wzh.daria6918.cn

[R58] 下载文件
来源：http://mgk.vqdsnc.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ijb.yuxming.cn

[R59] 发 POST JSON
来源：http://hry.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vyc.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://gkj.ywan-chungtsiang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uui.yfazqb.com

[R61] 磁盘占用
来源：http://cth.nanxinkj.top

df -h;  du -sh *
来源：http://dcp.chenzaomai.com

[R62] 找最占空间的文件
来源：http://ybp.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://psy.zdbjq.cn

[R63] 内存与进程
来源：http://ouu.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://icl.shuidangran.top

[R64] 结束进程
来源：http://kkp.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://huh.uphjek.com

[R65] 查看端口占用
来源：http://llj.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://map.snrcjt.cn

[R66] 定时任务
来源：http://gyc.dianchejie.cn

crontab -e;  crontab -l
来源：http://xoq.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://xmj.tian-w.cn

openssl rand -hex 16
来源：http://nnu.nanxinkj.top

[R68] 计算文件校验值
来源：http://dds.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://kqx.yj202588.top

[R69] 生成随机密码
来源：http://czr.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://jpu.jyoumei.cn

[R70] 时间戳与互转
来源：http://drf.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://bcr.sysykeji.top

[R71] 日期格式化
来源：http://nai.9152youxi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tch.meibo888.top

[R72] 等待端口就绪
来源：http://ekb.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uqf.yj20258888.top

[R73] 分割大日志
来源：http://sxb.fktsv.cn

split -l 1000 big.log part_
来源：http://ecv.redwolf501.top

[R74] 批量重命名
来源：http://mqr.hammf.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kbl.nanxinkj.top

[R75] 导出环境变量
来源：http://zyk.ehwqpu.com

export PATH="$HOME/bin:$PATH"
来源：http://sur.ybcxt.top

[R76] 使用临时文件
来源：http://qcw.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://krd.daxiang520.top

[R77] 读取用户输入
来源：http://zgk.dashuyun.cn

read -rp "请输入: " ans
来源：http://nlw.fzhhl.top

[R78] 交互式菜单
来源：http://lri.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://vuk.zhoulong.xyz

[R79] 解析命令行选项
来源：http://mwk.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://thi.uphjek.com

[R80] 查看脚本执行耗时
来源：http://aqd.cheryme.top

time ./run.sh
来源：http://orz.shuidangran.top

================================================================================
来源：http://cst.nanxuanxn.top

S. C / C++ 专题
来源：http://tiq.9152youxi.cn

================================================================================
来源：http://bti.birdmap.top

[S01] C：Hello World
来源：http://hge.zhijiandao.cn

#include <stdio.h>
来源：http://khc.xinyue.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://wcv.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://dvh.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://utr.dianchejie.cn

[S03] C：读入整数
来源：http://rht.birdmap.top

int x; scanf("%d", &x);
来源：http://kiz.zycfv.cn

[S04] C：字符串复制
来源：http://bzs.guowangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://jtt.52xcode.cn

[S05] C：字符串长度
来源：http://dfd.jinghuilouyu.cn

strlen(s)
来源：http://dlk.gotoacloud.top

[S06] C：字符串比较
来源：http://oqb.9152youxi.cn

strcmp(a, b) == 0
来源：http://ssw.zycfv.cn

[S07] C：数组遍历求和
来源：http://erf.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://aak.yj20258.top

[S08] C：动态内存分配与释放
来源：http://raw.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wqd.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://snw.zhoulong.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nux.yj20258.top

[S10] C：指针与解引用
来源：http://vrx.yuxming.cn

int *p = &a;  *p = 5;
来源：http://siw.cqqwz.cn

[S11] C：逐行读文件
来源：http://kdw.sufxvd.cn


<!-- 参考信息 -->