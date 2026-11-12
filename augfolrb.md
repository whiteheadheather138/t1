代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://tqm.daxiang520.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://fvd.ydjk.org.cn

[Q43] 标量子查询
来源：http://gla.dashuyun.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://byh.vqdsnc.cn

[Q44] IN 子查询
来源：http://pij.zhengqikj.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://spr.zhongyouzk.top

[Q45] EXISTS 判断存在
来源：http://gef.yj202588.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bpp.c1oappe.top

[Q46] NOT EXISTS 判断不存在
来源：http://srs.hongshengwenyu.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://jvv.ivvv.top

[Q47] 与平均值比较
来源：http://epb.gaohongyu789.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://azo.cashguo.top

[Q48] CTE 公用表表达式
来源：http://ain.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cft.ehwqpu.com

SELECT * FROM t WHERE c > 5;
来源：http://drn.vqdsnc.cn

[Q49] 更新单行
来源：http://vtx.sufxvd.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uej.gzhubu.top

[Q50] 批量更新
来源：http://sjg.hesvh.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ckq.guannengcc.top

[Q51] 用子查询更新
来源：http://kvr.smart0.xyz

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://waw.gzhubu.top

[Q52] 删除指定行
来源：http://hdl.quarkkingdee.top

DELETE FROM users WHERE id = 10;
来源：http://qzc.xuetiantiany.cn

[Q53] 按条件删除
来源：http://lmn.ctjpmb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xbx.yfazqb.com

[Q54] 清空表
来源：http://fnh.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://zah.xziqi.cn

[Q55] 排名（并列占位）
来源：http://vwv.hnxiangtu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ozq.jinqigfzy.top

[Q56] 密集排名（并列不占位）
来源：http://nfs.havefunace.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wea.zhiwuduotai.top

[Q57] 行号
来源：http://hjn.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cdw.zhijiandao.cn

[Q58] 累计求和
来源：http://rme.zycfv.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qkt.ehwqpu.com

[Q59] 分组内累计
来源：http://ynl.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://whs.gogol.net.cn

[Q60] 取上一行 / 下一行
来源：http://xgy.jinqigfzy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vie.yonumen.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zws.shanyushiyangtech.top

[Q61] 移动平均
来源：http://pgl.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uqc.ywan-chungtsiang.top

[Q62] 分组占比
来源：http://eog.zhoulong.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hsp.redwolf501.top

[Q63] 开启事务
来源：http://pqr.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://pxe.jinqigfzy.top

[Q64] 提交事务
来源：http://dpb.hywenlv.cn

COMMIT;
来源：http://mqf.shzxlz.cn

[Q65] 回滚事务
来源：http://jyj.zhaomingkeji.xyz

ROLLBACK;
来源：http://oea.hysaishi.cn

[Q66] 行锁查询
来源：http://jlu.yuanzhike.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://boe.iojbl.cn

[Q67] 设置隔离级别
来源：http://eit.jinqigfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bsq.zhaomingkeji.xyz

[Q68] 保存点
来源：http://wna.cheryme.top

SAVEPOINT sp1;
来源：http://kqs.bjfxy.top

ROLLBACK TO sp1;
来源：http://exv.yvedp.cn

[Q69] 查看执行计划
来源：http://ypv.bbcook.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://xrq.bjfxy.top

[Q70] 更新统计信息
来源：http://roi.gzhubu.top

ANALYZE TABLE users;
来源：http://jpz.guowangkeji.top

[Q71] 查看建表语句
来源：http://sig.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://jrb.xinyue.icu

[Q72] 查看索引
来源：http://fpi.yj20258.top

SHOW INDEX FROM users;
来源：http://oxe.sysykeji.top

[Q73] 查看表状态
来源：http://cey.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://udh.tarul.cn

[Q74] 强制使用索引
来源：http://rdk.cashguo.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wsz.nanxuanxn.top

[Q75] 日期格式化
来源：http://vrd.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wvm.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lpi.gotoacloud.top

[Q76] 按天统计
来源：http://czx.aizwys.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://svt.vehdjk.com

[Q77] 时间加减
来源：http://tfu.yonumen.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vhv.redwolf501.top

[Q78] 当前时间
来源：http://oqb.tarul.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nuk.nanxinkj.top

[Q79] 字符串拼接
来源：http://sjo.jlsjyb.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pon.yonumen.top

[Q80] 字符串截取
来源：http://mcv.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xne.zhengqikj.top

[Q81] 字符串替换
来源：http://npq.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vgq.cdnleiting.top

[Q82] 字符长度与字节长度
来源：http://aau.hnqzz.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zqn.xinyue.icu

[Q83] 大小写转换
来源：http://kpl.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mnt.ctjpmb.com

[Q84] 去除首尾空格
来源：http://eab.jqgfzy.top

SELECT TRIM(name) FROM users;
来源：http://hjd.316326.xyz

[Q85] 数值取整
来源：http://wsa.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ueo.uphjek.com

[Q86] 读取 JSON 字段
来源：http://hzy.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vif.birdmap.top

[Q87] JSON 字段做条件
来源：http://yek.shangyingyoupin.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xuo.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://tna.gogol.net.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ajj.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xzb.yfazqb.com

[Q89] 判断表是否存在
来源：http://qjm.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://llp.cucudq.cn

[Q90] 生成序号列
来源：http://zrx.nanxinkj.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://byd.xuetiantiany.cn

================================================================================
来源：http://bta.daria6918.cn

R. Bash 专题
来源：http://sdf.cdnleiting.top

================================================================================
来源：http://ffo.fanxiaobao.xyz

[R01] shebang 与严格模式
来源：http://dfm.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://rit.shuidangran.top

set -euo pipefail
来源：http://sie.iojbl.cn

[R02] 变量赋值与使用
来源：http://zop.tanke756.top

name="Tom"; echo "$name"
来源：http://irf.jianghu66.top

[R03] 只读变量
来源：http://mrz.daria6918.cn

readonly PI=3.14
来源：http://giz.shanyushiyangkeji.top

[R04] 位置参数
来源：http://ikl.c1oappe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nls.mhx1999.top

[R05] 参数默认值
来源：http://emf.uphjek.com

name="${1:-default}"
来源：http://qfi.sufxvd.cn

[R06] 判断命令是否存在
来源：http://qxs.gaohongyu789.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sow.xuetiantiany.cn

[R07] if 判断文件
来源：http://wxt.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xmh.shuidangran.top

[R08] 数值比较
来源：http://chl.nanxuanxn.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dwz.hnqzz.top

[R09] 字符串比较
来源：http://kwk.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xns.aizwys.cn

[R10] 正则匹配
来源：http://ytr.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rtr.hongshengwenyu.top

[R11] case 多分支
来源：http://wdx.gotoacloud.top

case "$1" in
来源：http://gnw.aizwys.cn

start) echo "启动" ;;
来源：http://tvn.316326.xyz

stop)  echo "停止" ;;
来源：http://uqz.mhx1999.top

*)     echo "未知命令" ;;
来源：http://tku.wangdashe.top

esac
来源：http://lpp.zhixingplan.top

[R12] for 遍历文件
来源：http://ksr.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://lky.sysykeji.top

[R13] for 计数循环
来源：http://nzu.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://abp.9152youxi.cn

[R14] C 风格 for
来源：http://izg.ivvv.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://egz.nanxinkj.top

[R15] while 逐行读文件
来源：http://cfl.hnxiangtu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qov.yj202588.top

[R16] until 等待条件
来源：http://xdb.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gut.wangshuangyany.cn

[R17] 数组定义与取值
来源：http://nua.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://myv.aizwys.cn

[R18] 遍历数组
来源：http://owu.yuanzhike.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zmw.bjfxy.top

[R19] 数组长度
来源：http://ugp.epnwcf.com

echo "${#arr[@]}"
来源：http://xva.fengsongda.top

[R20] 关联数组（字典）
来源：http://cml.aizwys.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oue.ybcxt.top

[R21] 字符串长度
来源：http://tgx.vqdsnc.cn

echo "${#s}"
来源：http://esn.dashuyun.cn

[R22] 截取子串
来源：http://ucj.tian-w.cn

echo "${s:0:5}"
来源：http://jjz.ydjk.org.cn

[R23] 字符串替换
来源：http://mpx.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://voq.hesvh.cn

[R24] 大小写转换
来源：http://brh.jlsjyb.cn

echo "${s^^}"; echo "${s,,}"
来源：http://tta.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://mne.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zzz.yvedp.cn

[R26] 命令替换
来源：http://yqp.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://kqw.havefunace.top

[R27] 算术展开
来源：http://qfo.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://vvn.quarkkingdee.top

[R28] 浮点运算
来源：http://rgx.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://nlm.bbcook.cn

[R29] 定义函数
来源：http://bmv.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kvj.hfpthk.cn

[R30] 函数返回状态码
来源：http://thn.fzhhl.top

f() { return 0; }; f || echo "失败了"
来源：http://smf.tian-w.cn

[R31] 局部变量
来源：http://zek.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://nyr.jiagoushi.top

[R32] 参数个数校验
来源：http://obb.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lww.shangyingyoupin.top

[R33] 捕获错误并提示行号
来源：http://rzp.fktsv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lsh.havefunace.top

[R34] 退出时清理
来源：http://dmx.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ihv.pycfn.com

[R35] 后台执行并等待
来源：http://kxw.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qdz.ydzc1.top

[R36] 并发执行多个任务
来源：http://zuw.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zvg.guowangkeji.top

[R37] 把输出赋给变量
来源：http://vwm.hammf.cn

files=$(ls -1)
来源：http://hew.hcnkem.com

[R38] 管道串联
来源：http://jra.ydjk.org.cn

cat a.txt | grep -i error | wc -l
来源：http://rso.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://xvi.hnxiangtu.top

cmd > out.log 2>&1
来源：http://pke.dashuyun.cn

[R40] 追加写日志
来源：http://qmm.guowangkeji.top

echo "log" >> out.log
来源：http://lbc.yvedp.cn

[R41] 丢弃输出
来源：http://nbt.yj20258888.top

cmd >/dev/null 2>&1
来源：http://gbr.hfpthk.cn

[R42] 输入重定向
来源：http://jxd.ywan-chungtsiang.top

wc -l < a.txt
来源：http://fil.fzhhl.top

[R43] 按名字查找文件
来源：http://ovj.iojbl.cn

find . -name "*.log" -type f
来源：http://diw.dashuyun.cn

[R44] 按修改时间查找
来源：http://bhw.yuanzhike.top

find . -mtime -7 -type f
来源：http://qoa.hongshengwenyu.top

[R45] 批量删除
来源：http://imv.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://sah.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://qgx.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qrv.yanxiufei.cn

[R47] sed 单行替换
来源：http://mbi.gaohongyu789.top

sed -i 's/foo/bar/g' a.txt
来源：http://qhz.nwbrower.top

[R48] awk 取指定列
来源：http://fhu.ivvv.top

awk '{print $1, $3}' a.txt
来源：http://ccc.hywenlv.cn

[R49] awk 带条件
来源：http://for.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rar.fktsv.cn

[R50] awk 求和
来源：http://zeb.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://kat.cqqwz.cn

[R51] 排序去重取前几
来源：http://hzg.zhiwuduotai.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dxf.zhiwuduotai.top

[R52] 统计行数
来源：http://dfq.epnwcf.com

wc -l a.txt
来源：http://xpo.yuxming.cn

[R53] 查看文件头与实时尾
来源：http://cxt.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fyt.birdmap.top

[R54] 比较两个文件
来源：http://tzo.jqgufenzy.top

diff a.txt b.txt
来源：http://yfu.haohaochexian.top

[R55] 压缩与解压
来源：http://obk.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xib.tianlin.xyz

[R56] 远程拷贝
来源：http://rdg.cheryme.top

scp file user@host:/path/
来源：http://cua.cqqwz.cn

[R57] 远程执行命令
来源：http://run.fehbvm.com

ssh user@host 'uptime'
来源：http://apl.zhiwuduotai.top

[R58] 下载文件
来源：http://oyr.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gbw.ctjpmb.com

[R59] 发 POST JSON
来源：http://imb.xylfe.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://znu.hysaishi.cn

[R60] 只看 HTTP 状态码
来源：http://vkr.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sua.sufxvd.cn

[R61] 磁盘占用
来源：http://qdc.ydzc1.top

df -h;  du -sh *
来源：http://aht.ivvv.top

[R62] 找最占空间的文件
来源：http://avr.bbcook.cn

du -ah . | sort -rh | head -10
来源：http://qtg.nanxuanxn.top

[R63] 内存与进程
来源：http://oxe.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://gka.tanke756.top

[R64] 结束进程
来源：http://ffk.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://hlw.birdmap.top

[R65] 查看端口占用
来源：http://izz.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dwo.ydjk.org.cn

[R66] 定时任务
来源：http://jqj.cqqwz.cn

crontab -e;  crontab -l
来源：http://vmt.sysykeji.top

[R67] 生成随机十六进制串
来源：http://zwi.xinyue.icu

openssl rand -hex 16
来源：http://kai.chenlongwang.top

[R68] 计算文件校验值
来源：http://riu.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://mbd.yfazqb.com

[R69] 生成随机密码
来源：http://gub.xuanzx.com

head -c 16 /dev/urandom | base64
来源：http://qbn.zhoulong.xyz

[R70] 时间戳与互转
来源：http://ptr.ybcxt.top

date +%s;  date -d @1700000000
来源：http://mfa.zhongyouzk.top

[R71] 日期格式化
来源：http://wyp.cashguo.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://zzq.hfpthk.cn

[R72] 等待端口就绪
来源：http://ufd.sysykeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ocr.zhoulong.xyz

[R73] 分割大日志
来源：http://mvn.quarkkingdee.top

split -l 1000 big.log part_
来源：http://wgt.xinyue.icu

[R74] 批量重命名
来源：http://rck.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://asx.pycfn.com

[R75] 导出环境变量
来源：http://wlo.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://szp.xylfe.cn

[R76] 使用临时文件
来源：http://lgu.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pqa.fzhhl.top

[R77] 读取用户输入
来源：http://kzv.cqqwz.cn

read -rp "请输入: " ans
来源：http://ibi.vehdjk.com

[R78] 交互式菜单
来源：http://lok.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://kwu.jinqigufen.top

[R79] 解析命令行选项
来源：http://amw.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cgk.hysaishi.cn

[R80] 查看脚本执行耗时
来源：http://qjn.hammf.cn

time ./run.sh
来源：http://vdn.zycfv.cn

================================================================================
来源：http://rwo.shuidangran.top

S. C / C++ 专题
来源：http://onl.sjlbkw.cn

================================================================================
来源：http://qxp.52xcode.cn

[S01] C：Hello World
来源：http://dmn.zdqjudy.top

#include <stdio.h>
来源：http://iox.daria6918.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vfi.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://fxi.c1oappe.top

int a = 10; printf("%d\n", a);
来源：http://rgw.sufxvd.cn

[S03] C：读入整数
来源：http://lio.shangyingyoupin.top

int x; scanf("%d", &x);
来源：http://izz.nanxuanxn.top

[S04] C：字符串复制
来源：http://rhs.jqgufenzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://fmu.aizwys.cn

[S05] C：字符串长度
来源：http://sxq.hammf.cn

strlen(s)
来源：http://brb.xinyue.icu

[S06] C：字符串比较
来源：http://quc.nanxinkj.top

strcmp(a, b) == 0
来源：http://zua.mhx1999.top

[S07] C：数组遍历求和
来源：http://vzj.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sto.c1oappe.top

[S08] C：动态内存分配与释放
来源：http://lod.svipenyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ito.fehbvm.com

[S09] C：结构体定义与初始化
来源：http://bud.meibo888.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zsm.fktsv.cn

[S10] C：指针与解引用
来源：http://ngp.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://dgr.guannengcc.top

[S11] C：逐行读文件
来源：http://sip.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://tnd.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lfj.cashguo.top

fclose(f);
来源：http://edw.316326.xyz

[S12] C：写文件
来源：http://knq.svipenyu.cn


<!-- 参考信息 -->