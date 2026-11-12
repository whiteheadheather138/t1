代发 wailian999

SELECT o.id, u.name, p.title FROM orders o
来源：http://bpr.xuetiantiany.cn

JOIN users u ON u.id = o.user_id
来源：http://tzn.shanyushiyangtech.top

JOIN products p ON p.id = o.product_id;
来源：http://iqh.chenzaomai.com

[Q42] 连接条件附加过滤
来源：http://zpb.xuetiantiany.cn

SELECT u.name, o.amount FROM users u
来源：http://prw.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://njk.hongshengwenyu.top

[Q43] 标量子查询
来源：http://ksm.fzhhl.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://shs.jinqigufen.top

[Q44] IN 子查询
来源：http://dmz.uphjek.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://qhv.dianchejie.cn

[Q45] EXISTS 判断存在
来源：http://axf.xuanzx.com

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zdo.nwbrower.top

[Q46] NOT EXISTS 判断不存在
来源：http://wct.vqdsnc.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dkf.zhiwuduotai.top

[Q47] 与平均值比较
来源：http://xhe.9152youxi.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://qxa.redwolf501.top

[Q48] CTE 公用表表达式
来源：http://mjh.hywenlv.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qnu.cheryme.top

SELECT * FROM t WHERE c > 5;
来源：http://vho.nwbrower.top

[Q49] 更新单行
来源：http://vlx.sjlbkw.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dbx.gogol.net.cn

[Q50] 批量更新
来源：http://qbi.shangyingyoupin.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://nyl.jqgufenzy.top

[Q51] 用子查询更新
来源：http://uuz.yonumen.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://era.iojbl.cn

[Q52] 删除指定行
来源：http://pwh.ehwqpu.com

DELETE FROM users WHERE id = 10;
来源：http://xlb.hfpthk.cn

[Q53] 按条件删除
来源：http://ymo.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rdt.jlsjyb.cn

[Q54] 清空表
来源：http://tcw.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://evk.xylfe.cn

[Q55] 排名（并列占位）
来源：http://fkv.yanxiufei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://lph.shuidangran.top

[Q56] 密集排名（并列不占位）
来源：http://tfe.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gfr.xuanzx.com

[Q57] 行号
来源：http://eou.sweek.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avs.zhongyouzk.top

[Q58] 累计求和
来源：http://rbz.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://evw.kuanghao11.cn

[Q59] 分组内累计
来源：http://xmo.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://olt.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://kwc.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pyy.smart0.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xwn.hysaishi.cn

[Q61] 移动平均
来源：http://rww.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cxt.tian-w.cn

[Q62] 分组占比
来源：http://fxe.ivvv.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xjq.havefunace.top

[Q63] 开启事务
来源：http://ndp.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://zme.yj20258.top

[Q64] 提交事务
来源：http://ndj.shzxlz.cn

COMMIT;
来源：http://xzt.snrcjt.cn

[Q65] 回滚事务
来源：http://mku.zdbjq.cn

ROLLBACK;
来源：http://zsd.bjfxy.top

[Q66] 行锁查询
来源：http://zlo.havefunace.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cje.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://llg.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qzy.52xcode.cn

[Q68] 保存点
来源：http://bfq.andypj.xyz

SAVEPOINT sp1;
来源：http://xjo.zdqjudy.top

ROLLBACK TO sp1;
来源：http://aka.52xcode.cn

[Q69] 查看执行计划
来源：http://ghc.52xcode.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hon.hfpthk.cn

[Q70] 更新统计信息
来源：http://bkv.snrcjt.cn

ANALYZE TABLE users;
来源：http://ttt.hammf.cn

[Q71] 查看建表语句
来源：http://vhq.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iri.xuetiantiany.cn

[Q72] 查看索引
来源：http://bat.yj202588.top

SHOW INDEX FROM users;
来源：http://swb.hongshengwenyu.top

[Q73] 查看表状态
来源：http://gzy.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vcl.quarkkingdee.top

[Q74] 强制使用索引
来源：http://ujg.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://fnv.yvedp.cn

[Q75] 日期格式化
来源：http://vux.hysaishi.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://glz.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xzc.xziqi.cn

[Q76] 按天统计
来源：http://alw.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zyc.hcnkem.com

[Q77] 时间加减
来源：http://sdp.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wdm.snrcjt.cn

[Q78] 当前时间
来源：http://ugd.wangdashe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://oxc.iojbl.cn

[Q79] 字符串拼接
来源：http://zsb.bjfxy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://aft.zhixingplan.top

[Q80] 字符串截取
来源：http://xxn.fanxiaobao.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jci.jianghu66.top

[Q81] 字符串替换
来源：http://slc.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://oha.yfazqb.com

[Q82] 字符长度与字节长度
来源：http://ftm.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fni.c1oappe.top

[Q83] 大小写转换
来源：http://beu.bbcook.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jlg.xuetiantiany.cn

[Q84] 去除首尾空格
来源：http://kgs.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://yuv.dianchejie.cn

[Q85] 数值取整
来源：http://luj.shuidangran.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zhe.yj20258.top

[Q86] 读取 JSON 字段
来源：http://nkm.chenzaomai.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ksj.cheryme.top

[Q87] JSON 字段做条件
来源：http://xzv.316326.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://maw.nanxuanxn.top

[Q88] 行转列（条件聚合）
来源：http://ayy.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wya.guowangkeji.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jky.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://ndk.cdnleiting.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iqp.andypj.xyz

[Q90] 生成序号列
来源：http://zph.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bry.yj20258888.top

================================================================================
来源：http://kzp.guannengcc.top

R. Bash 专题
来源：http://gah.c1oappe.top

================================================================================
来源：http://wui.yj202588.top

[R01] shebang 与严格模式
来源：http://fui.yj20258.top

#!/usr/bin/env bash
来源：http://hfi.shangyingyoupin.top

set -euo pipefail
来源：http://wkc.jqgfzy.top

[R02] 变量赋值与使用
来源：http://ggr.hesvh.cn

name="Tom"; echo "$name"
来源：http://imc.jiagoushi.top

[R03] 只读变量
来源：http://mwm.ybcxt.top

readonly PI=3.14
来源：http://yft.zhengqikj.top

[R04] 位置参数
来源：http://tlu.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ycb.gzhubu.top

[R05] 参数默认值
来源：http://poi.fzhhl.top

name="${1:-default}"
来源：http://cwb.yongpay.top

[R06] 判断命令是否存在
来源：http://lgb.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://aen.sweek.top

[R07] if 判断文件
来源：http://lin.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xdk.sufxvd.cn

[R08] 数值比较
来源：http://qoz.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://kku.dianchejie.cn

[R09] 字符串比较
来源：http://ahv.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gvo.jlsjyb.cn

[R10] 正则匹配
来源：http://ccw.xuanzx.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nlk.mhx1999.top

[R11] case 多分支
来源：http://str.tianlin.xyz

case "$1" in
来源：http://ref.yueranfly.top

start) echo "启动" ;;
来源：http://bph.daria6918.cn

stop)  echo "停止" ;;
来源：http://yig.aizwys.cn

*)     echo "未知命令" ;;
来源：http://zfh.zhiwuduotai.top

esac
来源：http://yto.cashguo.top

[R12] for 遍历文件
来源：http://bmc.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://bcm.yj20258888.top

[R13] for 计数循环
来源：http://kkj.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://fbo.yangfankeji.com

[R14] C 风格 for
来源：http://hle.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://upf.hywenlv.cn

[R15] while 逐行读文件
来源：http://jew.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bom.fzhhl.top

[R16] until 等待条件
来源：http://qvg.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qmy.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://agx.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://ckp.yonumen.top

[R18] 遍历数组
来源：http://bib.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kus.fzhhl.top

[R19] 数组长度
来源：http://use.quarkkingdee.top

echo "${#arr[@]}"
来源：http://oye.zhixingplan.top

[R20] 关联数组（字典）
来源：http://krl.smart0.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rfa.sjlbkw.cn

[R21] 字符串长度
来源：http://pvb.yangfankeji.com

echo "${#s}"
来源：http://jlv.tian-w.cn

[R22] 截取子串
来源：http://hev.fengsongda.top

echo "${s:0:5}"
来源：http://vrr.zhijiandao.cn

[R23] 字符串替换
来源：http://zrp.zhiwuduotai.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ngc.pengpengdd.cyou

[R24] 大小写转换
来源：http://ikg.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://wnj.zdbjq.cn

[R25] 去后缀 / 去前缀
来源：http://atr.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://roz.gotoacloud.top

[R26] 命令替换
来源：http://rev.cashguo.top

now=$(date +%F); echo "$now"
来源：http://kll.yueranfly.top

[R27] 算术展开
来源：http://ouh.mhx1999.top

echo $((1 + 2 * 3))
来源：http://oye.sufxvd.cn

[R28] 浮点运算
来源：http://ley.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://avn.yj20258888.top

[R29] 定义函数
来源：http://ehv.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gsp.dianchejie.cn

[R30] 函数返回状态码
来源：http://xra.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://mnl.daria6918.cn

[R31] 局部变量
来源：http://grk.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://fux.zhoulong.xyz

[R32] 参数个数校验
来源：http://mqm.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uji.ehwqpu.com

[R33] 捕获错误并提示行号
来源：http://vbg.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xku.xuanzx.com

[R34] 退出时清理
来源：http://zvr.yvedp.cn

trap 'rm -f "$tmp"' EXIT
来源：http://kkq.tianlin.xyz

[R35] 后台执行并等待
来源：http://pae.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yzm.bbcook.cn

[R36] 并发执行多个任务
来源：http://gpq.ydzc1.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kgo.fzhhl.top

[R37] 把输出赋给变量
来源：http://kgw.zdbjq.cn

files=$(ls -1)
来源：http://bnd.hfpthk.cn

[R38] 管道串联
来源：http://kpk.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://sbp.ydjk.org.cn

[R39] 重定向标准输出与错误
来源：http://ysu.cqqwz.cn

cmd > out.log 2>&1
来源：http://mmv.daria6918.cn

[R40] 追加写日志
来源：http://kki.pengpengdd.cyou

echo "log" >> out.log
来源：http://pqm.andypj.xyz

[R41] 丢弃输出
来源：http://gis.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://oyk.jiagoushi.top

[R42] 输入重定向
来源：http://akq.jinyuanbaomall.cn

wc -l < a.txt
来源：http://jai.hnxiangtu.top

[R43] 按名字查找文件
来源：http://jwn.bbcook.cn

find . -name "*.log" -type f
来源：http://ewx.sysykeji.top

[R44] 按修改时间查找
来源：http://eja.sjlbkw.cn

find . -mtime -7 -type f
来源：http://zvb.ydjk.org.cn

[R45] 批量删除
来源：http://ond.fktsv.cn

find . -name "*.tmp" -delete
来源：http://wek.wangdashe.top

[R46] 递归替换文件内容
来源：http://bvm.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bso.0kj1m.cn

[R47] sed 单行替换
来源：http://lfo.yfazqb.com

sed -i 's/foo/bar/g' a.txt
来源：http://oqn.kuanghao11.cn

[R48] awk 取指定列
来源：http://hfq.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://pxx.xziqi.cn

[R49] awk 带条件
来源：http://ksh.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xkl.jqgufenzy.top

[R50] awk 求和
来源：http://qsz.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://cjq.fktsv.cn

[R51] 排序去重取前几
来源：http://dly.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://qzo.hfpthk.cn

[R52] 统计行数
来源：http://zkf.ivvv.top

wc -l a.txt
来源：http://tos.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://ebj.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ebl.iojbl.cn

[R54] 比较两个文件
来源：http://ive.jianghu66.top

diff a.txt b.txt
来源：http://xzx.52xcode.cn

[R55] 压缩与解压
来源：http://iqy.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nkw.yj20258888.top

[R56] 远程拷贝
来源：http://trj.andypj.xyz

scp file user@host:/path/
来源：http://qsi.wangshuangyany.cn

[R57] 远程执行命令
来源：http://lmc.mhx1999.top

ssh user@host 'uptime'
来源：http://uql.feifeiyinyue.top

[R58] 下载文件
来源：http://pwc.guowangkeji.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ydv.zhixingplan.top

[R59] 发 POST JSON
来源：http://qco.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ooi.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://dhx.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://taj.uphjek.com

[R61] 磁盘占用
来源：http://aiu.shanyushiyangtech.top

df -h;  du -sh *
来源：http://xkc.gzhubu.top

[R62] 找最占空间的文件
来源：http://qrt.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://lko.guannengcc.top

[R63] 内存与进程
来源：http://zxs.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://edo.ydjk.org.cn

[R64] 结束进程
来源：http://mcz.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://hie.0kj1m.cn

[R65] 查看端口占用
来源：http://glv.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://afi.fanxiaobao.xyz

[R66] 定时任务
来源：http://dol.havefunace.top

crontab -e;  crontab -l
来源：http://cvt.hesvh.cn

[R67] 生成随机十六进制串
来源：http://fen.yongpay.top

openssl rand -hex 16
来源：http://xfs.cdnleiting.top

[R68] 计算文件校验值
来源：http://bew.ydjk.org.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iwi.chenzaomai.com

[R69] 生成随机密码
来源：http://sre.ydzc1.top

head -c 16 /dev/urandom | base64
来源：http://afe.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://jlb.fzhhl.top

date +%s;  date -d @1700000000
来源：http://zae.aibaodan.cn

[R71] 日期格式化
来源：http://psn.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://epe.yvedp.cn

[R72] 等待端口就绪
来源：http://tfv.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kat.hysaishi.cn

[R73] 分割大日志
来源：http://zgg.xziqi.cn

split -l 1000 big.log part_
来源：http://djz.zhijiandao.cn

[R74] 批量重命名
来源：http://scr.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nlj.kuanghao11.cn

[R75] 导出环境变量
来源：http://ayi.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://qyd.ybcxt.top

[R76] 使用临时文件
来源：http://btj.fzhhl.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jpn.tarul.cn

[R77] 读取用户输入
来源：http://hpc.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://mod.yanxiufei.cn

[R78] 交互式菜单
来源：http://uli.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pjm.pycfn.com

[R79] 解析命令行选项
来源：http://uan.shanyushiyangtech.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yix.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://nic.zhongyouzk.top

time ./run.sh
来源：http://kco.jinqigfzy.top

================================================================================
来源：http://nlo.hongshengwenyu.top

S. C / C++ 专题
来源：http://ijs.chenzaomai.com

================================================================================
来源：http://rfs.fengsongda.top

[S01] C：Hello World
来源：http://swz.0kj1m.cn

#include <stdio.h>
来源：http://ede.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wmq.tanke756.top

[S02] C：变量与格式化输出
来源：http://ktf.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://egt.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://upo.jiagoushi.top

int x; scanf("%d", &x);
来源：http://ojn.jianghu66.top

[S04] C：字符串复制
来源：http://pwz.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://qql.zhixingplan.top

[S05] C：字符串长度
来源：http://tao.yj20258.top

strlen(s)
来源：http://lzk.yuxming.cn

[S06] C：字符串比较
来源：http://dsq.hywenlv.cn

strcmp(a, b) == 0
来源：http://gyt.bbcook.cn

[S07] C：数组遍历求和
来源：http://thy.feifeiyinyue.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://urt.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://iic.chenjidiqi.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vak.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://rau.jinqigfzy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://llt.redwolf501.top

[S10] C：指针与解引用
来源：http://etc.wangdashe.top

int *p = &a;  *p = 5;
来源：http://gsg.fktsv.cn

[S11] C：逐行读文件
来源：http://owy.zhijiandao.cn


<!-- 参考信息 -->