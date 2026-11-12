代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qia.aizwys.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://lbp.sjlbkw.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://cic.daria6918.cn

[Q41] 多表连接
来源：http://xis.daxiang520.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://syv.shzxlz.cn

JOIN users u ON u.id = o.user_id
来源：http://yvf.iojbl.cn

JOIN products p ON p.id = o.product_id;
来源：http://cnp.hongshengwenyu.top

[Q42] 连接条件附加过滤
来源：http://rcl.hesvh.cn

SELECT u.name, o.amount FROM users u
来源：http://ffw.havefunace.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pmy.zhaomingkeji.xyz

[Q43] 标量子查询
来源：http://lic.jqgufenzy.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zim.cdnleiting.top

[Q44] IN 子查询
来源：http://mos.c1oappe.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yeo.pycfn.com

[Q45] EXISTS 判断存在
来源：http://psy.zdqjudy.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zly.hongshengwenyu.top

[Q46] NOT EXISTS 判断不存在
来源：http://xyu.zhongyouzk.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://gkl.pengpengdd.cyou

[Q47] 与平均值比较
来源：http://wxz.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://soz.wangdashe.top

[Q48] CTE 公用表表达式
来源：http://pdz.daria6918.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://sab.zhongyouzk.top

SELECT * FROM t WHERE c > 5;
来源：http://oja.ivvv.top

[Q49] 更新单行
来源：http://riy.wangshuangyany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mob.ehwqpu.com

[Q50] 批量更新
来源：http://keb.fanxiaobao.xyz

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://tem.c1oappe.top

[Q51] 用子查询更新
来源：http://ynh.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ftr.hongshengwenyu.top

[Q52] 删除指定行
来源：http://bvl.zhaomingkeji.xyz

DELETE FROM users WHERE id = 10;
来源：http://xks.gogol.net.cn

[Q53] 按条件删除
来源：http://kvf.aizwys.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dbf.ehwqpu.com

[Q54] 清空表
来源：http://fha.gogol.net.cn

TRUNCATE TABLE logs;
来源：http://tis.nwbrower.top

[Q55] 排名（并列占位）
来源：http://nsq.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpt.jinqigufen.top

[Q56] 密集排名（并列不占位）
来源：http://ntk.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sdh.ydzc1.top

[Q57] 行号
来源：http://zbs.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://jeb.epnwcf.com

[Q58] 累计求和
来源：http://xwx.yangfankeji.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ekg.mhx1999.top

[Q59] 分组内累计
来源：http://fae.epnwcf.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vtf.yueranfly.top

[Q60] 取上一行 / 下一行
来源：http://qov.aibaodan.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zvf.sxryk.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xsw.feifeiyinyue.top

[Q61] 移动平均
来源：http://ntp.redwolf501.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hns.uphjek.com

[Q62] 分组占比
来源：http://zal.jqgufenzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vyu.shzxlz.cn

[Q63] 开启事务
来源：http://pum.yj202588.top

START TRANSACTION;                -- 或 BEGIN
来源：http://qdb.nanxinkj.top

[Q64] 提交事务
来源：http://ikw.yj20258888.top

COMMIT;
来源：http://pzj.c1oappe.top

[Q65] 回滚事务
来源：http://wgs.quarkkingdee.top

ROLLBACK;
来源：http://yyw.havefunace.top

[Q66] 行锁查询
来源：http://jwy.zdbjq.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pew.mhx1999.top

[Q67] 设置隔离级别
来源：http://jpw.sysykeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yqk.guannengcc.top

[Q68] 保存点
来源：http://qji.shuidangran.top

SAVEPOINT sp1;
来源：http://qta.aizwys.cn

ROLLBACK TO sp1;
来源：http://vhm.sjlbkw.cn

[Q69] 查看执行计划
来源：http://mpt.zhongyouzk.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lbe.xuetiantiany.cn

[Q70] 更新统计信息
来源：http://puw.zhoulong.xyz

ANALYZE TABLE users;
来源：http://zeh.sufxvd.cn

[Q71] 查看建表语句
来源：http://fzx.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vjm.gotoacloud.top

[Q72] 查看索引
来源：http://uuy.9152youxi.cn

SHOW INDEX FROM users;
来源：http://wep.hcnkem.com

[Q73] 查看表状态
来源：http://wgs.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ddp.zhoulong.xyz

[Q74] 强制使用索引
来源：http://ecl.sxryk.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kre.hywenlv.cn

[Q75] 日期格式化
来源：http://aqj.yanxiufei.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dos.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eip.daxiang520.top

[Q76] 按天统计
来源：http://jpv.jinyuanbaomall.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rdo.shzxlz.cn

[Q77] 时间加减
来源：http://ulk.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mhl.dianchejie.cn

[Q78] 当前时间
来源：http://mim.ydjk.org.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wdc.meibo888.top

[Q79] 字符串拼接
来源：http://udj.yuxming.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://nar.havefunace.top

[Q80] 字符串截取
来源：http://cfi.yfazqb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ilq.jinqigfzy.top

[Q81] 字符串替换
来源：http://fow.epnwcf.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://twx.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://bka.dianchejie.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kqf.xuanzx.com

[Q83] 大小写转换
来源：http://rbu.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qsd.hfpthk.cn

[Q84] 去除首尾空格
来源：http://vxs.cashguo.top

SELECT TRIM(name) FROM users;
来源：http://vpa.svipenyu.cn

[Q85] 数值取整
来源：http://lrt.sweek.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://whi.jinyuanbaomall.cn

[Q86] 读取 JSON 字段
来源：http://qst.ydjk.org.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://erv.fzhhl.top

[Q87] JSON 字段做条件
来源：http://vee.mhx1999.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://cqo.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://fcx.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qcp.xuanzx.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://cny.guowangkeji.top

[Q89] 判断表是否存在
来源：http://igx.pengpengdd.cyou

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zik.9152youxi.cn

[Q90] 生成序号列
来源：http://ghs.shzxlz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wxh.fktsv.cn

================================================================================
来源：http://cbd.shuidangran.top

R. Bash 专题
来源：http://kut.jqgufenzy.top

================================================================================
来源：http://iul.hongshengwenyu.top

[R01] shebang 与严格模式
来源：http://jfp.fzhhl.top

#!/usr/bin/env bash
来源：http://dht.hysaishi.cn

set -euo pipefail
来源：http://xtg.ivvv.top

[R02] 变量赋值与使用
来源：http://ndy.jyoumei.cn

name="Tom"; echo "$name"
来源：http://dey.fengsongda.top

[R03] 只读变量
来源：http://yez.andypj.xyz

readonly PI=3.14
来源：http://wyv.quarkkingdee.top

[R04] 位置参数
来源：http://ubr.jinqigfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mvf.sxryk.cn

[R05] 参数默认值
来源：http://pgt.haohaochexian.top

name="${1:-default}"
来源：http://rzq.sweek.top

[R06] 判断命令是否存在
来源：http://hfm.c1oappe.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://zlh.nanxinkj.top

[R07] if 判断文件
来源：http://zma.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vcl.zhengqikj.top

[R08] 数值比较
来源：http://anh.vqdsnc.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pxl.aibaodan.cn

[R09] 字符串比较
来源：http://elk.sjlbkw.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fne.xylfe.cn

[R10] 正则匹配
来源：http://gah.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dcz.shangyingyoupin.top

[R11] case 多分支
来源：http://dvy.zhiwuduotai.top

case "$1" in
来源：http://kux.fengsongda.top

start) echo "启动" ;;
来源：http://mot.bjfxy.top

stop)  echo "停止" ;;
来源：http://krf.nwbrower.top

*)     echo "未知命令" ;;
来源：http://fst.zhongyouzk.top

esac
来源：http://oyg.pengpengdd.cyou

[R12] for 遍历文件
来源：http://grm.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://jez.svipenyu.cn

[R13] for 计数循环
来源：http://ghc.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://xmz.fengsongda.top

[R14] C 风格 for
来源：http://yur.nanxinkj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://znw.chenlongwang.top

[R15] while 逐行读文件
来源：http://pkp.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://izf.hysaishi.cn

[R16] until 等待条件
来源：http://fed.zhijiandao.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blp.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://oxi.xuetiantiany.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vhs.smart0.xyz

[R18] 遍历数组
来源：http://dvp.tarul.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gze.cucudq.cn

[R19] 数组长度
来源：http://dgx.tanke756.top

echo "${#arr[@]}"
来源：http://glf.316326.xyz

[R20] 关联数组（字典）
来源：http://ugg.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tfn.vehdjk.com

[R21] 字符串长度
来源：http://prx.yueranfly.top

echo "${#s}"
来源：http://jma.vehdjk.com

[R22] 截取子串
来源：http://xoc.jinyuanbaomall.cn

echo "${s:0:5}"
来源：http://iqz.316326.xyz

[R23] 字符串替换
来源：http://qtl.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qsp.chenzaomai.com

[R24] 大小写转换
来源：http://rwc.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://exq.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://hko.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jdw.gogol.net.cn

[R26] 命令替换
来源：http://pgn.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://rtn.yuanzhike.top

[R27] 算术展开
来源：http://ohc.pycfn.com

echo $((1 + 2 * 3))
来源：http://oii.shzxlz.cn

[R28] 浮点运算
来源：http://ejw.hcnkem.com

echo "scale=2; 10/3" | bc
来源：http://lmu.tarul.cn

[R29] 定义函数
来源：http://sve.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jit.vqdsnc.cn

[R30] 函数返回状态码
来源：http://bul.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://jae.havefunace.top

[R31] 局部变量
来源：http://idm.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://ppl.ctjpmb.com

[R32] 参数个数校验
来源：http://rny.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://msg.jiagoushi.top

[R33] 捕获错误并提示行号
来源：http://scf.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cri.daxiang520.top

[R34] 退出时清理
来源：http://pov.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://pss.xinyue.icu

[R35] 后台执行并等待
来源：http://xcs.sweek.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vby.mhx1999.top

[R36] 并发执行多个任务
来源：http://kzb.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xvm.gogol.net.cn

[R37] 把输出赋给变量
来源：http://vqw.fehbvm.com

files=$(ls -1)
来源：http://fui.sufxvd.cn

[R38] 管道串联
来源：http://sfo.xinyue.icu

cat a.txt | grep -i error | wc -l
来源：http://axa.bbcook.cn

[R39] 重定向标准输出与错误
来源：http://vte.hcnkem.com

cmd > out.log 2>&1
来源：http://oci.vqdsnc.cn

[R40] 追加写日志
来源：http://cwz.hnxiangtu.top

echo "log" >> out.log
来源：http://sza.fzhhl.top

[R41] 丢弃输出
来源：http://dqq.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://jte.nanxuanxn.top

[R42] 输入重定向
来源：http://wqx.wangshuangyany.cn

wc -l < a.txt
来源：http://sjo.gogol.net.cn

[R43] 按名字查找文件
来源：http://xhv.ydjk.org.cn

find . -name "*.log" -type f
来源：http://ewg.yuanzhike.top

[R44] 按修改时间查找
来源：http://qih.chenlongwang.top

find . -mtime -7 -type f
来源：http://rvj.wangshuangyany.cn

[R45] 批量删除
来源：http://beg.zhaomingkeji.xyz

find . -name "*.tmp" -delete
来源：http://ubv.0kj1m.cn

[R46] 递归替换文件内容
来源：http://svu.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xne.gogol.net.cn

[R47] sed 单行替换
来源：http://hlv.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://rrf.sweek.top

[R48] awk 取指定列
来源：http://ixy.shuidangran.top

awk '{print $1, $3}' a.txt
来源：http://nyo.yvedp.cn

[R49] awk 带条件
来源：http://onj.zhengqikj.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vph.shanyushiyangtech.top

[R50] awk 求和
来源：http://poc.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://acq.xziqi.cn

[R51] 排序去重取前几
来源：http://apy.vehdjk.com

sort a.txt | uniq -c | sort -rn | head
来源：http://cll.sysykeji.top

[R52] 统计行数
来源：http://dhx.zdbjq.cn

wc -l a.txt
来源：http://gcy.snrcjt.cn

[R53] 查看文件头与实时尾
来源：http://pby.hcnkem.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gwc.tianlin.xyz

[R54] 比较两个文件
来源：http://rmu.yfazqb.com

diff a.txt b.txt
来源：http://oaj.zhixingplan.top

[R55] 压缩与解压
来源：http://jmc.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qpu.havefunace.top

[R56] 远程拷贝
来源：http://pwo.aizwys.cn

scp file user@host:/path/
来源：http://mtc.xylfe.cn

[R57] 远程执行命令
来源：http://fzh.jinqigfzy.top

ssh user@host 'uptime'
来源：http://qcu.yuanzhike.top

[R58] 下载文件
来源：http://gtb.hnxiangtu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ayb.xziqi.cn

[R59] 发 POST JSON
来源：http://obp.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eub.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://tup.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://swg.jinyuanbaomall.cn

[R61] 磁盘占用
来源：http://gal.shangyingyoupin.top

df -h;  du -sh *
来源：http://vjy.epnwcf.com

[R62] 找最占空间的文件
来源：http://yan.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://exx.zhixingplan.top

[R63] 内存与进程
来源：http://zge.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://rnf.gogol.net.cn

[R64] 结束进程
来源：http://lbn.xuanzx.com

kill -9 $(pgrep -f app.py)
来源：http://xhi.bjfxy.top

[R65] 查看端口占用
来源：http://npo.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fcj.jiagoushi.top

[R66] 定时任务
来源：http://isg.cdnleiting.top

crontab -e;  crontab -l
来源：http://pxc.pengpengdd.cyou

[R67] 生成随机十六进制串
来源：http://org.kuanghao11.cn

openssl rand -hex 16
来源：http://ngr.cqqwz.cn

[R68] 计算文件校验值
来源：http://tvf.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hmt.jinqigfzy.top

[R69] 生成随机密码
来源：http://vzh.zhiwuduotai.top

head -c 16 /dev/urandom | base64
来源：http://ebz.9152youxi.cn

[R70] 时间戳与互转
来源：http://jph.0kj1m.cn

date +%s;  date -d @1700000000
来源：http://bco.guowangkeji.top

[R71] 日期格式化
来源：http://lqm.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lss.guannengcc.top

[R72] 等待端口就绪
来源：http://vjf.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xqi.haohaochexian.top

[R73] 分割大日志
来源：http://uqy.ybcxt.top

split -l 1000 big.log part_
来源：http://ogb.yangfankeji.com

[R74] 批量重命名
来源：http://zzt.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jze.jinyuanbaomall.cn

[R75] 导出环境变量
来源：http://zqj.uphjek.com

export PATH="$HOME/bin:$PATH"
来源：http://qyu.yj202588.top

[R76] 使用临时文件
来源：http://adb.yfazqb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fys.fengsongda.top

[R77] 读取用户输入
来源：http://nwo.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://hkx.chenjidiqi.icu

[R78] 交互式菜单
来源：http://jnd.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://eyr.chenzaomai.com

[R79] 解析命令行选项
来源：http://edl.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lko.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://qsi.yuanzhike.top

time ./run.sh
来源：http://xlg.nanxinkj.top

================================================================================
来源：http://srm.zhengqikj.top

S. C / C++ 专题
来源：http://kxs.yj202588.top

================================================================================
来源：http://gmo.xuanzx.com

[S01] C：Hello World
来源：http://fct.zdqjudy.top

#include <stdio.h>
来源：http://qkn.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ziy.gzhubu.top

[S02] C：变量与格式化输出
来源：http://zhw.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://mbf.hongshengwenyu.top

[S03] C：读入整数
来源：http://ykd.jinqigufen.top

int x; scanf("%d", &x);
来源：http://iga.daria6918.cn

[S04] C：字符串复制
来源：http://cxk.smart0.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://jtd.smart0.xyz

[S05] C：字符串长度
来源：http://nsm.jiagoushi.top

strlen(s)
来源：http://wfy.iojbl.cn

[S06] C：字符串比较
来源：http://arl.tian-w.cn

strcmp(a, b) == 0
来源：http://mvq.bjfxy.top

[S07] C：数组遍历求和
来源：http://ehh.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://swn.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://kff.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kdn.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://yhk.ybcxt.top


<!-- 参考信息 -->