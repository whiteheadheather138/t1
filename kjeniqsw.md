代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://azd.shangyingyoupin.top

JOIN users u ON u.id = o.user_id
来源：http://khp.smart0.xyz

JOIN products p ON p.id = o.product_id;
来源：http://cjt.epnwcf.com

[Q42] 连接条件附加过滤
来源：http://bbi.smart0.xyz

SELECT u.name, o.amount FROM users u
来源：http://kvf.dianchejie.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ovc.dianchejie.cn

[Q43] 标量子查询
来源：http://rog.yangfankeji.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://ujp.aibaodan.cn

[Q44] IN 子查询
来源：http://clt.yonumen.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://srn.shanyushiyangkeji.top

[Q45] EXISTS 判断存在
来源：http://rew.yuanzhike.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pnb.gogol.net.cn

[Q46] NOT EXISTS 判断不存在
来源：http://zxx.jqgufenzy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wdg.nanxinkj.top

[Q47] 与平均值比较
来源：http://mtr.tarul.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://cvw.sweek.top

[Q48] CTE 公用表表达式
来源：http://ikz.gotoacloud.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://spq.daria6918.cn

SELECT * FROM t WHERE c > 5;
来源：http://efe.tarul.cn

[Q49] 更新单行
来源：http://sqe.bbcook.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xjs.ydjk.org.cn

[Q50] 批量更新
来源：http://enf.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zld.dashuyun.cn

[Q51] 用子查询更新
来源：http://riq.fzhhl.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xyn.feifeiyinyue.top

[Q52] 删除指定行
来源：http://rrc.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://gdo.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://efe.hesvh.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fsu.svipenyu.cn

[Q54] 清空表
来源：http://lst.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://aiz.wangdashe.top

[Q55] 排名（并列占位）
来源：http://vmd.zhiwuduotai.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bsl.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://hmy.mhx1999.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jrg.haohaochexian.top

[Q57] 行号
来源：http://kan.aizwys.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://opr.shuidangran.top

[Q58] 累计求和
来源：http://mpa.feifeiyinyue.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ues.yj202588.top

[Q59] 分组内累计
来源：http://boh.uphjek.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nok.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://hsi.daxiang520.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zir.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rpr.haohaochexian.top

[Q61] 移动平均
来源：http://xnf.sweek.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ief.gotoacloud.top

[Q62] 分组占比
来源：http://jbw.tianlin.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gpw.c1oappe.top

[Q63] 开启事务
来源：http://fnv.hongshengwenyu.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pow.zdbjq.cn

[Q64] 提交事务
来源：http://gee.jqgfzy.top

COMMIT;
来源：http://wqr.daria6918.cn

[Q65] 回滚事务
来源：http://gev.fengsongda.top

ROLLBACK;
来源：http://ksn.0kj1m.cn

[Q66] 行锁查询
来源：http://baf.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zmy.fehbvm.com

[Q67] 设置隔离级别
来源：http://ehg.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wng.xinyue.icu

[Q68] 保存点
来源：http://lvi.hywenlv.cn

SAVEPOINT sp1;
来源：http://rzo.dashuyun.cn

ROLLBACK TO sp1;
来源：http://sgx.sysykeji.top

[Q69] 查看执行计划
来源：http://ahm.ydzc1.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://onr.vehdjk.com

[Q70] 更新统计信息
来源：http://njd.vqdsnc.cn

ANALYZE TABLE users;
来源：http://xft.nanxuanxn.top

[Q71] 查看建表语句
来源：http://xmi.ehwqpu.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mtq.birdmap.top

[Q72] 查看索引
来源：http://khk.hcnkem.com

SHOW INDEX FROM users;
来源：http://ylp.fzhhl.top

[Q73] 查看表状态
来源：http://sjt.xuetiantiany.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oup.havefunace.top

[Q74] 强制使用索引
来源：http://xix.andypj.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://obz.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://lqj.yangfankeji.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://etz.yongpay.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hmf.fzhhl.top

[Q76] 按天统计
来源：http://gyr.meibo888.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://akk.zhiwuduotai.top

[Q77] 时间加减
来源：http://tbh.cqqwz.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://att.0kj1m.cn

[Q78] 当前时间
来源：http://kwc.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://skb.hnqzz.top

[Q79] 字符串拼接
来源：http://tqb.cashguo.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bhz.nanxuanxn.top

[Q80] 字符串截取
来源：http://vib.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xdw.yj202588.top

[Q81] 字符串替换
来源：http://deh.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rik.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://pap.hnxiangtu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xbu.tianlin.xyz

[Q83] 大小写转换
来源：http://ran.yueranfly.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://usx.shuidangran.top

[Q84] 去除首尾空格
来源：http://caj.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://ixx.nanxinkj.top

[Q85] 数值取整
来源：http://qme.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://kbx.aibaodan.cn

[Q86] 读取 JSON 字段
来源：http://cwc.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kna.wangshuangyany.cn

[Q87] JSON 字段做条件
来源：http://hyh.birdmap.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ljy.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://ufv.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://koc.sysykeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tud.cheryme.top

[Q89] 判断表是否存在
来源：http://pfq.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tks.haohaochexian.top

[Q90] 生成序号列
来源：http://cit.cucudq.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qpc.ydjk.org.cn

================================================================================
来源：http://joc.feifeiyinyue.top

R. Bash 专题
来源：http://aih.hfpthk.cn

================================================================================
来源：http://jtp.ybcxt.top

[R01] shebang 与严格模式
来源：http://zef.hongshengwenyu.top

#!/usr/bin/env bash
来源：http://mmn.jqgufenzy.top

set -euo pipefail
来源：http://gfd.jqgufenzy.top

[R02] 变量赋值与使用
来源：http://tdd.svipenyu.cn

name="Tom"; echo "$name"
来源：http://xsn.quarkkingdee.top

[R03] 只读变量
来源：http://jgr.andypj.xyz

readonly PI=3.14
来源：http://kwl.ydjk.org.cn

[R04] 位置参数
来源：http://ksc.gogol.net.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pfk.tianlin.xyz

[R05] 参数默认值
来源：http://jly.jinqigufen.top

name="${1:-default}"
来源：http://cxs.aibaodan.cn

[R06] 判断命令是否存在
来源：http://ckh.smart0.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://asv.jinqigufen.top

[R07] if 判断文件
来源：http://jrq.shangyingyoupin.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cwz.shzxlz.cn

[R08] 数值比较
来源：http://cue.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ddg.jyoumei.cn

[R09] 字符串比较
来源：http://spx.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qjg.chenlongwang.top

[R10] 正则匹配
来源：http://yap.redwolf501.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bvs.vqdsnc.cn

[R11] case 多分支
来源：http://jij.dashuyun.cn

case "$1" in
来源：http://xux.sxryk.cn

start) echo "启动" ;;
来源：http://gbg.aibaodan.cn

stop)  echo "停止" ;;
来源：http://qrl.jinqigufen.top

*)     echo "未知命令" ;;
来源：http://ycw.hywenlv.cn

esac
来源：http://znw.pengpengdd.cyou

[R12] for 遍历文件
来源：http://pxu.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://akx.shangyingyoupin.top

[R13] for 计数循环
来源：http://lqq.9152youxi.cn

for i in {1..10}; do echo "$i"; done
来源：http://ine.svipenyu.cn

[R14] C 风格 for
来源：http://sqn.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bco.zycfv.cn

[R15] while 逐行读文件
来源：http://vnp.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wpl.fanxiaobao.xyz

[R16] until 等待条件
来源：http://vap.fzhhl.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rfu.sufxvd.cn

[R17] 数组定义与取值
来源：http://mlp.ybcxt.top

arr=(a b c); echo "${arr[0]}"
来源：http://tla.wangdashe.top

[R18] 遍历数组
来源：http://kik.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tyu.sweek.top

[R19] 数组长度
来源：http://ajc.redwolf501.top

echo "${#arr[@]}"
来源：http://dbh.aizwys.cn

[R20] 关联数组（字典）
来源：http://adf.xingfuxueyuan.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xwh.hnqzz.top

[R21] 字符串长度
来源：http://zll.jlsjyb.cn

echo "${#s}"
来源：http://ntw.quarkkingdee.top

[R22] 截取子串
来源：http://agq.hnqzz.top

echo "${s:0:5}"
来源：http://krh.smart0.xyz

[R23] 字符串替换
来源：http://jqq.jianghu66.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qkj.wangshuangyany.cn

[R24] 大小写转换
来源：http://vsm.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://oav.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://vgs.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jhp.cdnleiting.top

[R26] 命令替换
来源：http://pwr.dianchejie.cn

now=$(date +%F); echo "$now"
来源：http://wzm.tanke756.top

[R27] 算术展开
来源：http://ifi.52xcode.cn

echo $((1 + 2 * 3))
来源：http://hnr.xuetiantiany.cn

[R28] 浮点运算
来源：http://evw.zhixingplan.top

echo "scale=2; 10/3" | bc
来源：http://zmp.hesvh.cn

[R29] 定义函数
来源：http://cfa.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bfk.yanxiufei.cn

[R30] 函数返回状态码
来源：http://sqp.yvedp.cn

f() { return 0; }; f || echo "失败了"
来源：http://rgb.bjfxy.top

[R31] 局部变量
来源：http://hmc.epnwcf.com

f() { local x=1; echo "$x"; }
来源：http://hkv.haohaochexian.top

[R32] 参数个数校验
来源：http://pwz.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://csb.316326.xyz

[R33] 捕获错误并提示行号
来源：http://cvt.fzhhl.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xlr.guowangkeji.top

[R34] 退出时清理
来源：http://hsh.guowangkeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://fmz.gotoacloud.top

[R35] 后台执行并等待
来源：http://hdz.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://whr.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://esp.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dmn.gaohongyu789.top

[R37] 把输出赋给变量
来源：http://den.zdqjudy.top

files=$(ls -1)
来源：http://fyg.nwbrower.top

[R38] 管道串联
来源：http://bdl.zhongyouzk.top

cat a.txt | grep -i error | wc -l
来源：http://can.ydzc1.top

[R39] 重定向标准输出与错误
来源：http://yob.ywan-chungtsiang.top

cmd > out.log 2>&1
来源：http://ngy.aibaodan.cn

[R40] 追加写日志
来源：http://mre.tarul.cn

echo "log" >> out.log
来源：http://clw.meibo888.top

[R41] 丢弃输出
来源：http://rej.zhongyouzk.top

cmd >/dev/null 2>&1
来源：http://gjt.yongpay.top

[R42] 输入重定向
来源：http://fus.yangfankeji.com

wc -l < a.txt
来源：http://ato.jianghu66.top

[R43] 按名字查找文件
来源：http://oit.ppjwa.cn

find . -name "*.log" -type f
来源：http://nuq.yuanzhike.top

[R44] 按修改时间查找
来源：http://nco.meibo888.top

find . -mtime -7 -type f
来源：http://ktb.chenjidiqi.icu

[R45] 批量删除
来源：http://odm.birdmap.top

find . -name "*.tmp" -delete
来源：http://ipe.svipenyu.cn

[R46] 递归替换文件内容
来源：http://vsv.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ahv.tarul.cn

[R47] sed 单行替换
来源：http://zfx.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://osy.yangfankeji.com

[R48] awk 取指定列
来源：http://glr.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://gmt.epnwcf.com

[R49] awk 带条件
来源：http://gbz.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pas.cheryme.top

[R50] awk 求和
来源：http://odk.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://kss.yuanzhike.top

[R51] 排序去重取前几
来源：http://upe.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iew.hcnkem.com

[R52] 统计行数
来源：http://rmb.cqqwz.cn

wc -l a.txt
来源：http://jgo.yonumen.top

[R53] 查看文件头与实时尾
来源：http://cwj.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ryi.cashguo.top

[R54] 比较两个文件
来源：http://zaj.jinqigufen.top

diff a.txt b.txt
来源：http://jte.xuetiantiany.cn

[R55] 压缩与解压
来源：http://uzk.cdnleiting.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ycc.pengpengdd.cyou

[R56] 远程拷贝
来源：http://isq.fanxiaobao.xyz

scp file user@host:/path/
来源：http://jqd.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://ndq.sjlbkw.cn

ssh user@host 'uptime'
来源：http://tvy.wangshuangyany.cn

[R58] 下载文件
来源：http://gps.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lcb.yueranfly.top

[R59] 发 POST JSON
来源：http://nip.pengpengdd.cyou

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bof.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://bav.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mdn.fengsongda.top

[R61] 磁盘占用
来源：http://ttb.ydzc1.top

df -h;  du -sh *
来源：http://urw.ybcxt.top

[R62] 找最占空间的文件
来源：http://vva.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://xix.uphjek.com

[R63] 内存与进程
来源：http://rfs.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://wbs.epnwcf.com

[R64] 结束进程
来源：http://oyq.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://mie.yonumen.top

[R65] 查看端口占用
来源：http://fgz.gzhubu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rum.haohaochexian.top

[R66] 定时任务
来源：http://jhs.chenlongwang.top

crontab -e;  crontab -l
来源：http://tpp.xuetiantiany.cn

[R67] 生成随机十六进制串
来源：http://jea.ivvv.top

openssl rand -hex 16
来源：http://oqq.chenjidiqi.icu

[R68] 计算文件校验值
来源：http://mum.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://brl.jinqigufen.top

[R69] 生成随机密码
来源：http://ycs.tarul.cn

head -c 16 /dev/urandom | base64
来源：http://ohi.zhixingplan.top

[R70] 时间戳与互转
来源：http://rxq.daria6918.cn

date +%s;  date -d @1700000000
来源：http://qsu.tianlin.xyz

[R71] 日期格式化
来源：http://zav.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jab.jiagoushi.top

[R72] 等待端口就绪
来源：http://yrm.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://trk.fktsv.cn

[R73] 分割大日志
来源：http://wwr.birdmap.top

split -l 1000 big.log part_
来源：http://lpf.birdmap.top

[R74] 批量重命名
来源：http://lss.ivvv.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sdx.xinyue.icu

[R75] 导出环境变量
来源：http://hrq.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://wsn.jinqigufen.top

[R76] 使用临时文件
来源：http://yui.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xfx.pengpengdd.cyou

[R77] 读取用户输入
来源：http://hwd.jinqigufen.top

read -rp "请输入: " ans
来源：http://okh.hammf.cn

[R78] 交互式菜单
来源：http://ksr.shangyingyoupin.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vof.tianlin.xyz

[R79] 解析命令行选项
来源：http://cbm.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zss.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://fou.zhixingplan.top

time ./run.sh
来源：http://hbs.quarkkingdee.top

================================================================================
来源：http://bjy.sweek.top

S. C / C++ 专题
来源：http://yij.sxryk.cn

================================================================================
来源：http://kdc.zhijiandao.cn

[S01] C：Hello World
来源：http://ayo.jinqigufen.top

#include <stdio.h>
来源：http://ivv.yuanzhike.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kaw.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://yhn.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://mdj.redwolf501.top

[S03] C：读入整数
来源：http://fnv.fengsongda.top

int x; scanf("%d", &x);
来源：http://zlq.zhiwuduotai.top

[S04] C：字符串复制
来源：http://yyf.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qix.fengsongda.top

[S05] C：字符串长度
来源：http://vmy.sxryk.cn

strlen(s)
来源：http://cta.bjfxy.top

[S06] C：字符串比较
来源：http://itk.aizwys.cn

strcmp(a, b) == 0
来源：http://dju.dianchejie.cn

[S07] C：数组遍历求和
来源：http://ths.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dfm.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://axr.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xvb.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://aul.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rdu.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://yyy.gotoacloud.top

int *p = &a;  *p = 5;
来源：http://bdj.andypj.xyz

[S11] C：逐行读文件
来源：http://bxy.ehwqpu.com


<!-- 参考信息 -->