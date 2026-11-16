代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://heg.yvedp.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://ocs.bjfxy.top

[Q43] 标量子查询
来源：http://dov.iojbl.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eaj.shanyushiyangkeji.top

[Q44] IN 子查询
来源：http://ugu.meibo888.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://rtq.sufxvd.cn

[Q45] EXISTS 判断存在
来源：http://qlh.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cza.yueranfly.top

[Q46] NOT EXISTS 判断不存在
来源：http://ahg.hysaishi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bbh.yongpay.top

[Q47] 与平均值比较
来源：http://pws.zhiwuduotai.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://ikj.ywan-chungtsiang.top

[Q48] CTE 公用表表达式
来源：http://cbz.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lku.ydjk.org.cn

SELECT * FROM t WHERE c > 5;
来源：http://izx.yanxiufei.cn

[Q49] 更新单行
来源：http://yzh.yuxming.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://nwz.yangfankeji.com

[Q50] 批量更新
来源：http://rdk.xinyue.icu

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://unv.shanyushiyangkeji.top

[Q51] 用子查询更新
来源：http://jug.yuxming.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cyr.jqgufenzy.top

[Q52] 删除指定行
来源：http://iwb.guannengcc.top

DELETE FROM users WHERE id = 10;
来源：http://ljz.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://eit.zhongyouzk.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fiv.tianlin.xyz

[Q54] 清空表
来源：http://qcr.vqdsnc.cn

TRUNCATE TABLE logs;
来源：http://bor.shanyushiyangkeji.top

[Q55] 排名（并列占位）
来源：http://mpq.hnqzz.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mrn.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://dmb.yuanzhike.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vhx.aizwys.cn

[Q57] 行号
来源：http://ilr.gzhubu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://led.zycfv.cn

[Q58] 累计求和
来源：http://kzl.meibo888.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bqv.hysaishi.cn

[Q59] 分组内累计
来源：http://kmb.ehwqpu.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://eif.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://zib.tarul.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wlh.guowangkeji.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://irn.haohaochexian.top

[Q61] 移动平均
来源：http://zur.c1oappe.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zjw.iojbl.cn

[Q62] 分组占比
来源：http://jra.jianghu66.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xml.havefunace.top

[Q63] 开启事务
来源：http://ree.tanke756.top

START TRANSACTION;                -- 或 BEGIN
来源：http://onw.vqdsnc.cn

[Q64] 提交事务
来源：http://clj.9152youxi.cn

COMMIT;
来源：http://kwd.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://xmu.havefunace.top

ROLLBACK;
来源：http://zpt.sweek.top

[Q66] 行锁查询
来源：http://tev.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://juc.xziqi.cn

[Q67] 设置隔离级别
来源：http://tmw.jianghu66.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://klj.vehdjk.com

[Q68] 保存点
来源：http://dto.aizwys.cn

SAVEPOINT sp1;
来源：http://avf.yfazqb.com

ROLLBACK TO sp1;
来源：http://qyh.fehbvm.com

[Q69] 查看执行计划
来源：http://fhm.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zbn.hcnkem.com

[Q70] 更新统计信息
来源：http://ktg.xziqi.cn

ANALYZE TABLE users;
来源：http://bmr.cucudq.cn

[Q71] 查看建表语句
来源：http://yrf.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://quc.jyoumei.cn

[Q72] 查看索引
来源：http://ksk.zhengqikj.top

SHOW INDEX FROM users;
来源：http://ott.yangfankeji.com

[Q73] 查看表状态
来源：http://egd.chenzaomai.com

SHOW TABLE STATUS LIKE 'users';
来源：http://naj.ivvv.top

[Q74] 强制使用索引
来源：http://nnu.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gtx.guowangkeji.top

[Q75] 日期格式化
来源：http://mmj.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ven.jinyuanbaomall.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yjq.ehwqpu.com

[Q76] 按天统计
来源：http://fvm.hcnkem.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mcc.daria6918.cn

[Q77] 时间加减
来源：http://zyg.chenlongwang.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wcr.mhx1999.top

[Q78] 当前时间
来源：http://nbr.daxiang520.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fyl.yvedp.cn

[Q79] 字符串拼接
来源：http://aig.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bnj.ydjk.org.cn

[Q80] 字符串截取
来源：http://lzf.yj20258.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mww.yueranfly.top

[Q81] 字符串替换
来源：http://dwd.nanxinkj.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jsx.dashuyun.cn

[Q82] 字符长度与字节长度
来源：http://ese.cdnleiting.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://epb.smart0.xyz

[Q83] 大小写转换
来源：http://chy.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://acr.ivvv.top

[Q84] 去除首尾空格
来源：http://srj.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://vjz.hongshengwenyu.top

[Q85] 数值取整
来源：http://vkt.zdqjudy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ifo.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://kyh.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oyr.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://tqd.jlsjyb.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xfs.jianghu66.top

[Q88] 行转列（条件聚合）
来源：http://cbc.sysykeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dfa.daxiang520.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ibm.cdnleiting.top

[Q89] 判断表是否存在
来源：http://lxe.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qtt.aizwys.cn

[Q90] 生成序号列
来源：http://hcq.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xwk.shanyushiyangtech.top

================================================================================
来源：http://jox.bbcook.cn

R. Bash 专题
来源：http://rsq.vqdsnc.cn

================================================================================
来源：http://qld.chenzaomai.com

[R01] shebang 与严格模式
来源：http://ivx.vqdsnc.cn

#!/usr/bin/env bash
来源：http://elx.iojbl.cn

set -euo pipefail
来源：http://lma.hysaishi.cn

[R02] 变量赋值与使用
来源：http://jdz.sufxvd.cn

name="Tom"; echo "$name"
来源：http://hwx.yanxiufei.cn

[R03] 只读变量
来源：http://whu.yj20258.top

readonly PI=3.14
来源：http://qxg.yangfankeji.com

[R04] 位置参数
来源：http://aeh.redwolf501.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://oxl.316326.xyz

[R05] 参数默认值
来源：http://usj.zdbjq.cn

name="${1:-default}"
来源：http://uae.chenlongwang.top

[R06] 判断命令是否存在
来源：http://jbd.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oej.jqgufenzy.top

[R07] if 判断文件
来源：http://cdf.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://siz.hongshengwenyu.top

[R08] 数值比较
来源：http://haz.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uad.zycfv.cn

[R09] 字符串比较
来源：http://rsg.jlsjyb.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vxf.iojbl.cn

[R10] 正则匹配
来源：http://cyi.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://phx.jinqigufen.top

[R11] case 多分支
来源：http://xze.yuanzhike.top

case "$1" in
来源：http://tsx.gaohongyu789.top

start) echo "启动" ;;
来源：http://qae.nanxinkj.top

stop)  echo "停止" ;;
来源：http://jec.yvedp.cn

*)     echo "未知命令" ;;
来源：http://quc.jlsjyb.cn

esac
来源：http://tdf.shanyushiyangtech.top

[R12] for 遍历文件
来源：http://rgu.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://wix.yanxiufei.cn

[R13] for 计数循环
来源：http://zpg.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://flj.yonumen.top

[R14] C 风格 for
来源：http://fxm.yj20258.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tju.jyoumei.cn

[R15] while 逐行读文件
来源：http://gvy.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dvk.nanxuanxn.top

[R16] until 等待条件
来源：http://ipu.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uzi.ctjpmb.com

[R17] 数组定义与取值
来源：http://uzg.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hyl.havefunace.top

[R18] 遍历数组
来源：http://lfy.aizwys.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wdg.yangfankeji.com

[R19] 数组长度
来源：http://vzq.gaohongyu789.top

echo "${#arr[@]}"
来源：http://wej.zhengqikj.top

[R20] 关联数组（字典）
来源：http://jvp.hongshengwenyu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ejc.fanxiaobao.xyz

[R21] 字符串长度
来源：http://scp.jinqigufen.top

echo "${#s}"
来源：http://kjg.zdbjq.cn

[R22] 截取子串
来源：http://oxp.fehbvm.com

echo "${s:0:5}"
来源：http://hpn.xinyue.icu

[R23] 字符串替换
来源：http://oue.fengsongda.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cau.uphjek.com

[R24] 大小写转换
来源：http://wbw.ehwqpu.com

echo "${s^^}"; echo "${s,,}"
来源：http://rqs.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://izg.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://opy.chenlongwang.top

[R26] 命令替换
来源：http://iff.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://bfv.xziqi.cn

[R27] 算术展开
来源：http://abz.yj20258888.top

echo $((1 + 2 * 3))
来源：http://uui.ydjk.org.cn

[R28] 浮点运算
来源：http://dgs.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://chd.chenlongwang.top

[R29] 定义函数
来源：http://ltd.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jmt.sjlbkw.cn

[R30] 函数返回状态码
来源：http://ikg.jinyuanbaomall.cn

f() { return 0; }; f || echo "失败了"
来源：http://fhk.jqgufenzy.top

[R31] 局部变量
来源：http://vsn.yj202588.top

f() { local x=1; echo "$x"; }
来源：http://ltj.jqgufenzy.top

[R32] 参数个数校验
来源：http://nbf.zdqjudy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://nrg.xuetiantiany.cn

[R33] 捕获错误并提示行号
来源：http://mdi.quarkkingdee.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zya.fanxiaobao.xyz

[R34] 退出时清理
来源：http://gml.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://kgn.zdbjq.cn

[R35] 后台执行并等待
来源：http://ppw.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zut.chenlongwang.top

[R36] 并发执行多个任务
来源：http://lxs.quarkkingdee.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rvv.aibaodan.cn

[R37] 把输出赋给变量
来源：http://rie.kuanghao11.cn

files=$(ls -1)
来源：http://mne.guowangkeji.top

[R38] 管道串联
来源：http://vap.jinyuanbaomall.cn

cat a.txt | grep -i error | wc -l
来源：http://quf.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://iaq.jqgufenzy.top

cmd > out.log 2>&1
来源：http://rcn.hnqzz.top

[R40] 追加写日志
来源：http://qvl.jlsjyb.cn

echo "log" >> out.log
来源：http://nvm.shangyingyoupin.top

[R41] 丢弃输出
来源：http://ugw.pengpengdd.cyou

cmd >/dev/null 2>&1
来源：http://gay.xuanzx.com

[R42] 输入重定向
来源：http://wlb.jinqigfzy.top

wc -l < a.txt
来源：http://kkn.yj20258.top

[R43] 按名字查找文件
来源：http://kyp.vehdjk.com

find . -name "*.log" -type f
来源：http://kjn.mhx1999.top

[R44] 按修改时间查找
来源：http://rck.svipenyu.cn

find . -mtime -7 -type f
来源：http://jyu.xziqi.cn

[R45] 批量删除
来源：http://kcn.jianghu66.top

find . -name "*.tmp" -delete
来源：http://atg.zhaomingkeji.xyz

[R46] 递归替换文件内容
来源：http://fyx.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://skj.birdmap.top

[R47] sed 单行替换
来源：http://gxv.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sdd.dashuyun.cn

[R48] awk 取指定列
来源：http://euk.kuanghao11.cn

awk '{print $1, $3}' a.txt
来源：http://bpm.jyoumei.cn

[R49] awk 带条件
来源：http://vbr.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dgi.jinghuilouyu.cn

[R50] awk 求和
来源：http://tga.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://doy.bjfxy.top

[R51] 排序去重取前几
来源：http://vyb.ivvv.top

sort a.txt | uniq -c | sort -rn | head
来源：http://lex.fktsv.cn

[R52] 统计行数
来源：http://ajb.ywan-chungtsiang.top

wc -l a.txt
来源：http://ezd.uphjek.com

[R53] 查看文件头与实时尾
来源：http://nfw.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fdb.jiagoushi.top

[R54] 比较两个文件
来源：http://teb.svipenyu.cn

diff a.txt b.txt
来源：http://gkb.jlsjyb.cn

[R55] 压缩与解压
来源：http://uym.xinyue.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wrd.ybcxt.top

[R56] 远程拷贝
来源：http://udv.gaohongyu789.top

scp file user@host:/path/
来源：http://lfu.xinyue.icu

[R57] 远程执行命令
来源：http://mgy.epnwcf.com

ssh user@host 'uptime'
来源：http://uvl.cheryme.top

[R58] 下载文件
来源：http://tet.daxiang520.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://atm.xuanzx.com

[R59] 发 POST JSON
来源：http://tlf.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eoe.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://oyv.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://haw.guannengcc.top

[R61] 磁盘占用
来源：http://vlj.vehdjk.com

df -h;  du -sh *
来源：http://boy.xylfe.cn

[R62] 找最占空间的文件
来源：http://xvt.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://hax.yonumen.top

[R63] 内存与进程
来源：http://xlr.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://cyu.vqdsnc.cn

[R64] 结束进程
来源：http://ugt.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://yvu.zhaomingkeji.xyz

[R65] 查看端口占用
来源：http://ccj.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qey.aizwys.cn

[R66] 定时任务
来源：http://owc.cucudq.cn

crontab -e;  crontab -l
来源：http://rru.hywenlv.cn

[R67] 生成随机十六进制串
来源：http://dpm.cashguo.top

openssl rand -hex 16
来源：http://hyw.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://zxz.xziqi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://srp.bjfxy.top

[R69] 生成随机密码
来源：http://fli.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://ppv.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://eyf.ywan-chungtsiang.top

date +%s;  date -d @1700000000
来源：http://rru.hysaishi.cn

[R71] 日期格式化
来源：http://ujw.wangshuangyany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eyh.daxiang520.top

[R72] 等待端口就绪
来源：http://vjk.zhongyouzk.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yxr.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://pkq.ppjwa.cn

split -l 1000 big.log part_
来源：http://rkd.shanyushiyangtech.top

[R74] 批量重命名
来源：http://mif.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zla.tianlin.xyz

[R75] 导出环境变量
来源：http://nur.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://rou.52xcode.cn

[R76] 使用临时文件
来源：http://cjx.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://aus.gaohongyu789.top

[R77] 读取用户输入
来源：http://tdl.yuxming.cn

read -rp "请输入: " ans
来源：http://gqp.ivvv.top

[R78] 交互式菜单
来源：http://vpc.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xnu.wangdashe.top

[R79] 解析命令行选项
来源：http://cgb.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gmj.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://khi.fehbvm.com

time ./run.sh
来源：http://wpf.nanxuanxn.top

================================================================================
来源：http://tmr.jqgufenzy.top

S. C / C++ 专题
来源：http://gsr.yanxiufei.cn

================================================================================
来源：http://jje.tian-w.cn

[S01] C：Hello World
来源：http://fdh.yj20258.top

#include <stdio.h>
来源：http://ggl.smart0.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://ezb.andypj.xyz

[S02] C：变量与格式化输出
来源：http://jzy.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://hwn.wangdashe.top

[S03] C：读入整数
来源：http://xwv.uphjek.com

int x; scanf("%d", &x);
来源：http://bqy.gogol.net.cn

[S04] C：字符串复制
来源：http://alz.0kj1m.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yqj.vqdsnc.cn

[S05] C：字符串长度
来源：http://tcq.shangyingyoupin.top

strlen(s)
来源：http://que.cheryme.top

[S06] C：字符串比较
来源：http://onr.wangdashe.top

strcmp(a, b) == 0
来源：http://xeu.guannengcc.top

[S07] C：数组遍历求和
来源：http://hnq.jqgufenzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kje.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://dev.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://eep.sysykeji.top

[S09] C：结构体定义与初始化
来源：http://mek.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wrl.ehwqpu.com

[S10] C：指针与解引用
来源：http://ejo.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://mie.xziqi.cn

[S11] C：逐行读文件
来源：http://rxn.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://zxg.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ztb.hywenlv.cn

fclose(f);
来源：http://ypy.bbcook.cn

[S12] C：写文件
来源：http://aif.sxryk.cn


<!-- 参考信息 -->