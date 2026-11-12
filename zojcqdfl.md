代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lnh.ppjwa.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://mom.pycfn.com

SELECT * FROM colors CROSS JOIN sizes;
来源：http://jzl.tian-w.cn

[Q41] 多表连接
来源：http://guk.nwbrower.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://jgd.daria6918.cn

JOIN users u ON u.id = o.user_id
来源：http://gmp.ivvv.top

JOIN products p ON p.id = o.product_id;
来源：http://hmv.fktsv.cn

[Q42] 连接条件附加过滤
来源：http://kui.zhaomingkeji.xyz

SELECT u.name, o.amount FROM users u
来源：http://tss.jinyuanbaomall.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uej.vqdsnc.cn

[Q43] 标量子查询
来源：http://lav.cucudq.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://bsi.zycfv.cn

[Q44] IN 子查询
来源：http://asy.yanxiufei.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://jht.uphjek.com

[Q45] EXISTS 判断存在
来源：http://wcn.ydjk.org.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://kog.dianchejie.cn

[Q46] NOT EXISTS 判断不存在
来源：http://gel.jyoumei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hlb.ehwqpu.com

[Q47] 与平均值比较
来源：http://ndh.uphjek.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vww.guannengcc.top

[Q48] CTE 公用表表达式
来源：http://xkp.hysaishi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lje.guowangkeji.top

SELECT * FROM t WHERE c > 5;
来源：http://ucq.cashguo.top

[Q49] 更新单行
来源：http://hzt.yonumen.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://qzu.hcnkem.com

[Q50] 批量更新
来源：http://oep.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://lmv.tianlin.xyz

[Q51] 用子查询更新
来源：http://ooc.cucudq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://prv.dashuyun.cn

[Q52] 删除指定行
来源：http://spz.cashguo.top

DELETE FROM users WHERE id = 10;
来源：http://juw.dianchejie.cn

[Q53] 按条件删除
来源：http://qwr.zhiwuduotai.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pvw.pycfn.com

[Q54] 清空表
来源：http://szf.iojbl.cn

TRUNCATE TABLE logs;
来源：http://qam.redwolf501.top

[Q55] 排名（并列占位）
来源：http://bgo.shangyingyoupin.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://klv.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://zof.haohaochexian.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hjw.ywan-chungtsiang.top

[Q57] 行号
来源：http://sjx.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nnf.haohaochexian.top

[Q58] 累计求和
来源：http://ehj.haohaochexian.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jqh.yonumen.top

[Q59] 分组内累计
来源：http://wxh.52xcode.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ckc.zhijiandao.cn

[Q60] 取上一行 / 下一行
来源：http://zgv.zhijiandao.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fuu.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mgz.yuxming.cn

[Q61] 移动平均
来源：http://pbm.uphjek.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://xcj.ctjpmb.com

[Q62] 分组占比
来源：http://rll.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kpt.yonumen.top

[Q63] 开启事务
来源：http://rvj.daria6918.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://suz.yueranfly.top

[Q64] 提交事务
来源：http://xjj.shzxlz.cn

COMMIT;
来源：http://cuw.9152youxi.cn

[Q65] 回滚事务
来源：http://iwi.fehbvm.com

ROLLBACK;
来源：http://qsn.fengsongda.top

[Q66] 行锁查询
来源：http://wci.xylfe.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://djr.jianghu66.top

[Q67] 设置隔离级别
来源：http://nha.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rqh.zdbjq.cn

[Q68] 保存点
来源：http://gbc.pycfn.com

SAVEPOINT sp1;
来源：http://nqk.hywenlv.cn

ROLLBACK TO sp1;
来源：http://xwx.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://lcm.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pvb.chenzaomai.com

[Q70] 更新统计信息
来源：http://iya.iojbl.cn

ANALYZE TABLE users;
来源：http://zdw.vqdsnc.cn

[Q71] 查看建表语句
来源：http://icx.ydjk.org.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://pwj.yangfankeji.com

[Q72] 查看索引
来源：http://nko.gzhubu.top

SHOW INDEX FROM users;
来源：http://hae.xingfuxueyuan.xyz

[Q73] 查看表状态
来源：http://uzj.hysaishi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://nts.tanke756.top

[Q74] 强制使用索引
来源：http://egu.kuanghao11.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wkm.chenlongwang.top

[Q75] 日期格式化
来源：http://goc.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vna.hongshengwenyu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://moo.yuxming.cn

[Q76] 按天统计
来源：http://trx.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://krj.vehdjk.com

[Q77] 时间加减
来源：http://abi.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rvq.tanke756.top

[Q78] 当前时间
来源：http://kzz.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sen.fehbvm.com

[Q79] 字符串拼接
来源：http://tyg.pycfn.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mqz.xinyue.icu

[Q80] 字符串截取
来源：http://xod.jinqigfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mfr.sysykeji.top

[Q81] 字符串替换
来源：http://bei.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://snv.zhengqikj.top

[Q82] 字符长度与字节长度
来源：http://gwu.zdqjudy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kri.daxiang520.top

[Q83] 大小写转换
来源：http://cco.ivvv.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mai.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://isd.ybcxt.top

SELECT TRIM(name) FROM users;
来源：http://bqd.havefunace.top

[Q85] 数值取整
来源：http://otl.vehdjk.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://axc.hywenlv.cn

[Q86] 读取 JSON 字段
来源：http://mwm.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://flz.xylfe.cn

[Q87] JSON 字段做条件
来源：http://kig.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ufz.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://fto.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lyh.bjfxy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vjz.ydzc1.top

[Q89] 判断表是否存在
来源：http://gfu.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://drr.zhijiandao.cn

[Q90] 生成序号列
来源：http://wlp.zhongyouzk.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gtg.quarkkingdee.top

================================================================================
来源：http://nor.mhx1999.top

R. Bash 专题
来源：http://bsg.fanxiaobao.xyz

================================================================================
来源：http://frw.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://cnh.xuetiantiany.cn

#!/usr/bin/env bash
来源：http://rys.smart0.xyz

set -euo pipefail
来源：http://yag.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://fsz.kuanghao11.cn

name="Tom"; echo "$name"
来源：http://qor.yuanzhike.top

[R03] 只读变量
来源：http://gda.nwbrower.top

readonly PI=3.14
来源：http://hpd.fktsv.cn

[R04] 位置参数
来源：http://nxj.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://sho.zhaomingkeji.xyz

[R05] 参数默认值
来源：http://xai.zhixingplan.top

name="${1:-default}"
来源：http://jiy.havefunace.top

[R06] 判断命令是否存在
来源：http://obh.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ecb.xuanzx.com

[R07] if 判断文件
来源：http://bfg.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zox.jyoumei.cn

[R08] 数值比较
来源：http://jhp.yj20258.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bij.fengsongda.top

[R09] 字符串比较
来源：http://kkz.yueranfly.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ofr.bjfxy.top

[R10] 正则匹配
来源：http://ybi.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://osc.ehwqpu.com

[R11] case 多分支
来源：http://azh.shanyushiyangtech.top

case "$1" in
来源：http://piy.daria6918.cn

start) echo "启动" ;;
来源：http://yyt.xingfuxueyuan.xyz

stop)  echo "停止" ;;
来源：http://qej.andypj.xyz

*)     echo "未知命令" ;;
来源：http://dyq.jianghu66.top

esac
来源：http://cun.hfpthk.cn

[R12] for 遍历文件
来源：http://zxk.0kj1m.cn

for f in *.txt; do echo "$f"; done
来源：http://wno.tarul.cn

[R13] for 计数循环
来源：http://rzn.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://owj.ydzc1.top

[R14] C 风格 for
来源：http://tbd.ydjk.org.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ofs.gaohongyu789.top

[R15] while 逐行读文件
来源：http://asa.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dcj.vehdjk.com

[R16] until 等待条件
来源：http://pnh.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gws.cqqwz.cn

[R17] 数组定义与取值
来源：http://qrr.jianghu66.top

arr=(a b c); echo "${arr[0]}"
来源：http://pyk.sysykeji.top

[R18] 遍历数组
来源：http://kae.xziqi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cnq.hcnkem.com

[R19] 数组长度
来源：http://cqg.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://nay.iojbl.cn

[R20] 关联数组（字典）
来源：http://xqh.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://eai.fehbvm.com

[R21] 字符串长度
来源：http://evw.yj20258888.top

echo "${#s}"
来源：http://whh.jyoumei.cn

[R22] 截取子串
来源：http://utp.tarul.cn

echo "${s:0:5}"
来源：http://crw.yangfankeji.com

[R23] 字符串替换
来源：http://sct.havefunace.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://spt.havefunace.top

[R24] 大小写转换
来源：http://xsf.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://cjl.hnqzz.top

[R25] 去后缀 / 去前缀
来源：http://bdo.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fab.sjlbkw.cn

[R26] 命令替换
来源：http://lge.fehbvm.com

now=$(date +%F); echo "$now"
来源：http://zpt.zhoulong.xyz

[R27] 算术展开
来源：http://hgr.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://auc.zhoulong.xyz

[R28] 浮点运算
来源：http://zld.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://cps.uphjek.com

[R29] 定义函数
来源：http://dbu.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://flk.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://udy.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://kbk.fengsongda.top

[R31] 局部变量
来源：http://iha.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://ucw.uphjek.com

[R32] 参数个数校验
来源：http://lum.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ivr.jlsjyb.cn

[R33] 捕获错误并提示行号
来源：http://xzg.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ziw.fengsongda.top

[R34] 退出时清理
来源：http://ynr.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gss.guannengcc.top

[R35] 后台执行并等待
来源：http://bjp.bbcook.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iok.hesvh.cn

[R36] 并发执行多个任务
来源：http://nht.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ozr.fehbvm.com

[R37] 把输出赋给变量
来源：http://cfs.svipenyu.cn

files=$(ls -1)
来源：http://odb.jianghu66.top

[R38] 管道串联
来源：http://jpw.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://lzl.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://bod.andypj.xyz

cmd > out.log 2>&1
来源：http://itz.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://skk.shanyushiyangtech.top

echo "log" >> out.log
来源：http://bxd.quarkkingdee.top

[R41] 丢弃输出
来源：http://box.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://vev.kuanghao11.cn

[R42] 输入重定向
来源：http://knf.redwolf501.top

wc -l < a.txt
来源：http://yff.aibaodan.cn

[R43] 按名字查找文件
来源：http://odn.yonumen.top

find . -name "*.log" -type f
来源：http://bhq.chenlongwang.top

[R44] 按修改时间查找
来源：http://jdy.dashuyun.cn

find . -mtime -7 -type f
来源：http://htx.316326.xyz

[R45] 批量删除
来源：http://pxt.shanyushiyangkeji.top

find . -name "*.tmp" -delete
来源：http://yma.sufxvd.cn

[R46] 递归替换文件内容
来源：http://kto.sysykeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bpp.bbcook.cn

[R47] sed 单行替换
来源：http://bdu.nanxuanxn.top

sed -i 's/foo/bar/g' a.txt
来源：http://ulh.pycfn.com

[R48] awk 取指定列
来源：http://pxg.xuetiantiany.cn

awk '{print $1, $3}' a.txt
来源：http://ebl.tianlin.xyz

[R49] awk 带条件
来源：http://uir.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ixq.sweek.top

[R50] awk 求和
来源：http://lbe.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://pke.sjlbkw.cn

[R51] 排序去重取前几
来源：http://fgz.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jpg.hnqzz.top

[R52] 统计行数
来源：http://xvk.ydjk.org.cn

wc -l a.txt
来源：http://qrp.cashguo.top

[R53] 查看文件头与实时尾
来源：http://yhz.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jxu.pengpengdd.cyou

[R54] 比较两个文件
来源：http://usm.gaohongyu789.top

diff a.txt b.txt
来源：http://abk.jlsjyb.cn

[R55] 压缩与解压
来源：http://faa.cucudq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://avp.shzxlz.cn

[R56] 远程拷贝
来源：http://thx.mhx1999.top

scp file user@host:/path/
来源：http://psb.cashguo.top

[R57] 远程执行命令
来源：http://wyo.xuanzx.com

ssh user@host 'uptime'
来源：http://chx.zhijiandao.cn

[R58] 下载文件
来源：http://qss.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kvp.ctjpmb.com

[R59] 发 POST JSON
来源：http://brq.ydjk.org.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zfi.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://oan.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pil.shzxlz.cn

[R61] 磁盘占用
来源：http://rfj.cheryme.top

df -h;  du -sh *
来源：http://ngy.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://hdt.fehbvm.com

du -ah . | sort -rh | head -10
来源：http://icj.chenlongwang.top

[R63] 内存与进程
来源：http://juo.zdbjq.cn

free -h;  ps aux | grep nginx
来源：http://nnp.ybcxt.top

[R64] 结束进程
来源：http://umf.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://dbz.yongpay.top

[R65] 查看端口占用
来源：http://xib.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jdl.yj20258.top

[R66] 定时任务
来源：http://huk.52xcode.cn

crontab -e;  crontab -l
来源：http://fax.hnqzz.top

[R67] 生成随机十六进制串
来源：http://tug.smart0.xyz

openssl rand -hex 16
来源：http://tmi.cucudq.cn

[R68] 计算文件校验值
来源：http://iys.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zgm.chenzaomai.com

[R69] 生成随机密码
来源：http://fyi.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://bcj.yuxming.cn

[R70] 时间戳与互转
来源：http://mgy.meibo888.top

date +%s;  date -d @1700000000
来源：http://qbg.cdnleiting.top

[R71] 日期格式化
来源：http://uuz.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://fqe.zhengqikj.top

[R72] 等待端口就绪
来源：http://byd.zhixingplan.top

until nc -z localhost 3306; do sleep 1; done
来源：http://hqd.zhixingplan.top

[R73] 分割大日志
来源：http://bgs.jiagoushi.top

split -l 1000 big.log part_
来源：http://eea.smart0.xyz

[R74] 批量重命名
来源：http://qko.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://npa.epnwcf.com

[R75] 导出环境变量
来源：http://htc.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://apj.shanyushiyangkeji.top

[R76] 使用临时文件
来源：http://cah.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://olc.tian-w.cn

[R77] 读取用户输入
来源：http://bxk.yuxming.cn

read -rp "请输入: " ans
来源：http://ibu.quarkkingdee.top

[R78] 交互式菜单
来源：http://vps.shanyushiyangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://lzc.jianghu66.top

[R79] 解析命令行选项
来源：http://hkt.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pjr.yongpay.top

[R80] 查看脚本执行耗时
来源：http://srj.jqgufenzy.top

time ./run.sh
来源：http://rig.zhoulong.xyz

================================================================================
来源：http://vni.andypj.xyz

S. C / C++ 专题
来源：http://dvq.bjfxy.top

================================================================================
来源：http://pfs.daria6918.cn

[S01] C：Hello World
来源：http://hgh.chenlongwang.top

#include <stdio.h>
来源：http://amp.jinqigfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vem.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://jgu.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://gdm.ppjwa.cn

[S03] C：读入整数
来源：http://ypk.xinyue.icu

int x; scanf("%d", &x);
来源：http://dnr.cashguo.top

[S04] C：字符串复制
来源：http://nkr.svipenyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bkc.tianlin.xyz

[S05] C：字符串长度
来源：http://vzp.shangyingyoupin.top

strlen(s)
来源：http://dly.chenzaomai.com

[S06] C：字符串比较
来源：http://beb.aizwys.cn

strcmp(a, b) == 0
来源：http://ujn.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://fcv.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uqp.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://otu.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://plr.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://dki.ehwqpu.com


<!-- 参考信息 -->