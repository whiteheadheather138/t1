代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://zic.hysaishi.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://loo.kuanghao11.cn

[Q43] 标量子查询
来源：http://rwa.andypj.xyz

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zom.nanxuanxn.top

[Q44] IN 子查询
来源：http://xrk.yj20258888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://agq.haohaochexian.top

[Q45] EXISTS 判断存在
来源：http://cyg.mhx1999.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zbq.meibo888.top

[Q46] NOT EXISTS 判断不存在
来源：http://pzr.zdbjq.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://nio.bjfxy.top

[Q47] 与平均值比较
来源：http://whs.ctjpmb.com

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://way.zhiwuduotai.top

[Q48] CTE 公用表表达式
来源：http://uya.ehwqpu.com

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ypn.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://ztm.snrcjt.cn

[Q49] 更新单行
来源：http://exg.yj20258.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xfk.vehdjk.com

[Q50] 批量更新
来源：http://zan.sufxvd.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://cgu.tanke756.top

[Q51] 用子查询更新
来源：http://ker.c1oappe.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xqd.cheryme.top

[Q52] 删除指定行
来源：http://iqh.chenjidiqi.icu

DELETE FROM users WHERE id = 10;
来源：http://bfy.vqdsnc.cn

[Q53] 按条件删除
来源：http://snm.jinqigufen.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hen.smart0.xyz

[Q54] 清空表
来源：http://yqf.haohaochexian.top

TRUNCATE TABLE logs;
来源：http://mcs.redwolf501.top

[Q55] 排名（并列占位）
来源：http://iqj.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jeq.xingfuxueyuan.xyz

[Q56] 密集排名（并列不占位）
来源：http://jfe.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://fxd.jinqigfzy.top

[Q57] 行号
来源：http://byk.yj202588.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yuy.snrcjt.cn

[Q58] 累计求和
来源：http://zyw.zhixingplan.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://meu.sjlbkw.cn

[Q59] 分组内累计
来源：http://gki.nanxinkj.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://krk.nwbrower.top

[Q60] 取上一行 / 下一行
来源：http://ebd.gzhubu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vzs.zhongyouzk.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uqs.yj20258.top

[Q61] 移动平均
来源：http://pep.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://azz.jianghu66.top

[Q62] 分组占比
来源：http://qiu.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ktu.snrcjt.cn

[Q63] 开启事务
来源：http://gmj.tianlin.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cqf.nanxuanxn.top

[Q64] 提交事务
来源：http://kle.kuanghao11.cn

COMMIT;
来源：http://lwn.meibo888.top

[Q65] 回滚事务
来源：http://ggy.pycfn.com

ROLLBACK;
来源：http://xfi.zhiwuduotai.top

[Q66] 行锁查询
来源：http://nbn.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://vtf.zhoulong.xyz

[Q67] 设置隔离级别
来源：http://lwb.yanxiufei.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mab.jiagoushi.top

[Q68] 保存点
来源：http://djx.chenzaomai.com

SAVEPOINT sp1;
来源：http://ikc.52xcode.cn

ROLLBACK TO sp1;
来源：http://ont.hywenlv.cn

[Q69] 查看执行计划
来源：http://pny.daxiang520.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nrx.gotoacloud.top

[Q70] 更新统计信息
来源：http://hel.hysaishi.cn

ANALYZE TABLE users;
来源：http://ttz.meibo888.top

[Q71] 查看建表语句
来源：http://jar.yj202588.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fry.fzhhl.top

[Q72] 查看索引
来源：http://opk.chenzaomai.com

SHOW INDEX FROM users;
来源：http://rcj.gogol.net.cn

[Q73] 查看表状态
来源：http://npz.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ygk.cashguo.top

[Q74] 强制使用索引
来源：http://tez.hywenlv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sxr.daxiang520.top

[Q75] 日期格式化
来源：http://hzc.zycfv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mgp.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vto.9152youxi.cn

[Q76] 按天统计
来源：http://rkv.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://aye.iojbl.cn

[Q77] 时间加减
来源：http://jhz.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://idj.sjlbkw.cn

[Q78] 当前时间
来源：http://uup.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rld.hcnkem.com

[Q79] 字符串拼接
来源：http://tyu.gotoacloud.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wov.ppjwa.cn

[Q80] 字符串截取
来源：http://jfp.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bps.yj20258888.top

[Q81] 字符串替换
来源：http://kwx.shuidangran.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tjj.wangdashe.top

[Q82] 字符长度与字节长度
来源：http://srv.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dli.shuidangran.top

[Q83] 大小写转换
来源：http://uqk.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gkw.xinyue.icu

[Q84] 去除首尾空格
来源：http://kbf.zhoulong.xyz

SELECT TRIM(name) FROM users;
来源：http://pof.dashuyun.cn

[Q85] 数值取整
来源：http://fej.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zds.ydjk.org.cn

[Q86] 读取 JSON 字段
来源：http://gga.andypj.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zbm.andypj.xyz

[Q87] JSON 字段做条件
来源：http://ggo.xingfuxueyuan.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ozh.sxryk.cn

[Q88] 行转列（条件聚合）
来源：http://bzt.cashguo.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pcj.sjlbkw.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oms.quarkkingdee.top

[Q89] 判断表是否存在
来源：http://gho.zycfv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pmz.wangdashe.top

[Q90] 生成序号列
来源：http://thp.bbcook.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://atp.hnxiangtu.top

================================================================================
来源：http://oyd.jinqigfzy.top

R. Bash 专题
来源：http://whz.shangyingyoupin.top

================================================================================
来源：http://kme.vehdjk.com

[R01] shebang 与严格模式
来源：http://uhp.ivvv.top

#!/usr/bin/env bash
来源：http://hls.zhaomingkeji.xyz

set -euo pipefail
来源：http://qfs.xinyue.icu

[R02] 变量赋值与使用
来源：http://coz.shzxlz.cn

name="Tom"; echo "$name"
来源：http://hoi.pengpengdd.cyou

[R03] 只读变量
来源：http://hio.yvedp.cn

readonly PI=3.14
来源：http://ejw.yangfankeji.com

[R04] 位置参数
来源：http://xwh.jianghu66.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rqs.tanke756.top

[R05] 参数默认值
来源：http://gyh.yj20258.top

name="${1:-default}"
来源：http://wvu.quarkkingdee.top

[R06] 判断命令是否存在
来源：http://uwn.jiagoushi.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://efg.cqqwz.cn

[R07] if 判断文件
来源：http://vfk.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://buo.jqgufenzy.top

[R08] 数值比较
来源：http://yax.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://thd.yfazqb.com

[R09] 字符串比较
来源：http://gvu.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gew.sxryk.cn

[R10] 正则匹配
来源：http://rxp.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hok.gotoacloud.top

[R11] case 多分支
来源：http://ery.ybcxt.top

case "$1" in
来源：http://spf.fehbvm.com

start) echo "启动" ;;
来源：http://eco.yueranfly.top

stop)  echo "停止" ;;
来源：http://qcn.0kj1m.cn

*)     echo "未知命令" ;;
来源：http://ftj.shuidangran.top

esac
来源：http://tdx.zhaomingkeji.xyz

[R12] for 遍历文件
来源：http://hua.hcnkem.com

for f in *.txt; do echo "$f"; done
来源：http://lxb.guannengcc.top

[R13] for 计数循环
来源：http://luw.ehwqpu.com

for i in {1..10}; do echo "$i"; done
来源：http://rnt.zycfv.cn

[R14] C 风格 for
来源：http://svv.jiagoushi.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bzm.dashuyun.cn

[R15] while 逐行读文件
来源：http://rqs.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xxx.bbcook.cn

[R16] until 等待条件
来源：http://jqz.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zkr.xuetiantiany.cn

[R17] 数组定义与取值
来源：http://ywj.cheryme.top

arr=(a b c); echo "${arr[0]}"
来源：http://fqx.hongshengwenyu.top

[R18] 遍历数组
来源：http://uva.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nlz.xuetiantiany.cn

[R19] 数组长度
来源：http://yvu.fehbvm.com

echo "${#arr[@]}"
来源：http://kki.hnqzz.top

[R20] 关联数组（字典）
来源：http://zww.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jcf.fzhhl.top

[R21] 字符串长度
来源：http://fuw.yanxiufei.cn

echo "${#s}"
来源：http://zbq.fktsv.cn

[R22] 截取子串
来源：http://dyh.c1oappe.top

echo "${s:0:5}"
来源：http://yvv.yanxiufei.cn

[R23] 字符串替换
来源：http://pen.c1oappe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dlc.wangdashe.top

[R24] 大小写转换
来源：http://txt.jinqigufen.top

echo "${s^^}"; echo "${s,,}"
来源：http://qqg.316326.xyz

[R25] 去后缀 / 去前缀
来源：http://wti.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://bif.daria6918.cn

[R26] 命令替换
来源：http://fgt.yuanzhike.top

now=$(date +%F); echo "$now"
来源：http://kfa.chenjidiqi.icu

[R27] 算术展开
来源：http://hyn.zycfv.cn

echo $((1 + 2 * 3))
来源：http://qgh.zhengqikj.top

[R28] 浮点运算
来源：http://sub.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://tkw.shuidangran.top

[R29] 定义函数
来源：http://rql.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nqf.svipenyu.cn

[R30] 函数返回状态码
来源：http://xme.epnwcf.com

f() { return 0; }; f || echo "失败了"
来源：http://aop.shuidangran.top

[R31] 局部变量
来源：http://egg.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://ght.jinqigfzy.top

[R32] 参数个数校验
来源：http://adx.fanxiaobao.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hoj.fktsv.cn

[R33] 捕获错误并提示行号
来源：http://cwy.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vbf.shzxlz.cn

[R34] 退出时清理
来源：http://kjv.xuetiantiany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ywe.xziqi.cn

[R35] 后台执行并等待
来源：http://awf.ctjpmb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://loh.pengpengdd.cyou

[R36] 并发执行多个任务
来源：http://frw.yj20258888.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://psf.cheryme.top

[R37] 把输出赋给变量
来源：http://dmb.fktsv.cn

files=$(ls -1)
来源：http://yrm.birdmap.top

[R38] 管道串联
来源：http://doy.nwbrower.top

cat a.txt | grep -i error | wc -l
来源：http://asn.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://fum.shanyushiyangkeji.top

cmd > out.log 2>&1
来源：http://jxs.jinghuilouyu.cn

[R40] 追加写日志
来源：http://qra.kuanghao11.cn

echo "log" >> out.log
来源：http://umn.yanxiufei.cn

[R41] 丢弃输出
来源：http://eay.jqgfzy.top

cmd >/dev/null 2>&1
来源：http://shx.jianghu66.top

[R42] 输入重定向
来源：http://grb.nwbrower.top

wc -l < a.txt
来源：http://sbl.fktsv.cn

[R43] 按名字查找文件
来源：http://ojs.gogol.net.cn

find . -name "*.log" -type f
来源：http://rlb.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://aia.gaohongyu789.top

find . -mtime -7 -type f
来源：http://lmf.yanxiufei.cn

[R45] 批量删除
来源：http://rel.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://mrd.havefunace.top

[R46] 递归替换文件内容
来源：http://elh.hfpthk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iua.cashguo.top

[R47] sed 单行替换
来源：http://ytu.shzxlz.cn

sed -i 's/foo/bar/g' a.txt
来源：http://gdh.ydzc1.top

[R48] awk 取指定列
来源：http://pni.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://jux.zhongyouzk.top

[R49] awk 带条件
来源：http://cdy.ybcxt.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kdm.sxryk.cn

[R50] awk 求和
来源：http://bwm.0kj1m.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xmf.yj202588.top

[R51] 排序去重取前几
来源：http://cxu.cqqwz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://uec.iojbl.cn

[R52] 统计行数
来源：http://qfe.cqqwz.cn

wc -l a.txt
来源：http://dnb.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://lxt.aizwys.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ido.xinyue.icu

[R54] 比较两个文件
来源：http://tnl.shuidangran.top

diff a.txt b.txt
来源：http://oni.jyoumei.cn

[R55] 压缩与解压
来源：http://jfc.ivvv.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kvj.yuxming.cn

[R56] 远程拷贝
来源：http://uoz.zycfv.cn

scp file user@host:/path/
来源：http://eto.gaohongyu789.top

[R57] 远程执行命令
来源：http://tqo.tarul.cn

ssh user@host 'uptime'
来源：http://fub.ydjk.org.cn

[R58] 下载文件
来源：http://rgj.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zcy.gotoacloud.top

[R59] 发 POST JSON
来源：http://ayf.vqdsnc.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lfh.yongpay.top

[R60] 只看 HTTP 状态码
来源：http://yzg.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rrf.kuanghao11.cn

[R61] 磁盘占用
来源：http://pza.yj20258888.top

df -h;  du -sh *
来源：http://ojt.c1oappe.top

[R62] 找最占空间的文件
来源：http://isd.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://afq.316326.xyz

[R63] 内存与进程
来源：http://oeb.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://bjg.zhengqikj.top

[R64] 结束进程
来源：http://ekl.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://hqb.nanxinkj.top

[R65] 查看端口占用
来源：http://wrh.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lbv.hywenlv.cn

[R66] 定时任务
来源：http://ovk.gaohongyu789.top

crontab -e;  crontab -l
来源：http://jkv.hesvh.cn

[R67] 生成随机十六进制串
来源：http://epi.ydjk.org.cn

openssl rand -hex 16
来源：http://etf.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://gyl.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wpz.daxiang520.top

[R69] 生成随机密码
来源：http://ink.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://fcp.zhongyouzk.top

[R70] 时间戳与互转
来源：http://adn.tian-w.cn

date +%s;  date -d @1700000000
来源：http://emv.chenjidiqi.icu

[R71] 日期格式化
来源：http://pwf.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zwo.shanyushiyangtech.top

[R72] 等待端口就绪
来源：http://loj.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://mxt.hammf.cn

[R73] 分割大日志
来源：http://kpf.iojbl.cn

split -l 1000 big.log part_
来源：http://sia.ydjk.org.cn

[R74] 批量重命名
来源：http://rot.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wob.xingfuxueyuan.xyz

[R75] 导出环境变量
来源：http://zma.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://wwx.ivvv.top

[R76] 使用临时文件
来源：http://obd.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fvr.hcnkem.com

[R77] 读取用户输入
来源：http://bms.ehwqpu.com

read -rp "请输入: " ans
来源：http://nhv.svipenyu.cn

[R78] 交互式菜单
来源：http://xem.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://crh.ivvv.top

[R79] 解析命令行选项
来源：http://cfz.sufxvd.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dik.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://avt.shanyushiyangkeji.top

time ./run.sh
来源：http://nsh.pycfn.com

================================================================================
来源：http://fly.ppjwa.cn

S. C / C++ 专题
来源：http://mis.hcnkem.com

================================================================================
来源：http://zxc.hongshengwenyu.top

[S01] C：Hello World
来源：http://dyx.wangshuangyany.cn

#include <stdio.h>
来源：http://ofh.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://brx.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://ndh.ppjwa.cn

int a = 10; printf("%d\n", a);
来源：http://rzv.aizwys.cn

[S03] C：读入整数
来源：http://rko.ppjwa.cn

int x; scanf("%d", &x);
来源：http://mqb.gogol.net.cn

[S04] C：字符串复制
来源：http://qab.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pjk.nanxinkj.top

[S05] C：字符串长度
来源：http://dsa.9152youxi.cn

strlen(s)
来源：http://qip.snrcjt.cn

[S06] C：字符串比较
来源：http://zug.cucudq.cn

strcmp(a, b) == 0
来源：http://jrn.cheryme.top

[S07] C：数组遍历求和
来源：http://cwd.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rbq.ehwqpu.com

[S08] C：动态内存分配与释放
来源：http://vai.daxiang520.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fjf.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://zxp.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yyr.gzhubu.top

[S10] C：指针与解引用
来源：http://cdu.zdbjq.cn

int *p = &a;  *p = 5;
来源：http://muy.sufxvd.cn

[S11] C：逐行读文件
来源：http://ptg.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://rez.feifeiyinyue.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://gjg.daria6918.cn

fclose(f);
来源：http://fsl.jlsjyb.cn

[S12] C：写文件
来源：http://mve.vqdsnc.cn


<!-- 参考信息 -->