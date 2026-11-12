代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://bhi.jiagoushi.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://jou.andypj.xyz

[Q43] 标量子查询
来源：http://iyh.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://qnv.hywenlv.cn

[Q44] IN 子查询
来源：http://ehi.yj202588.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://quz.jlsjyb.cn

[Q45] EXISTS 判断存在
来源：http://yah.cheryme.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://bto.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://plh.wangdashe.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wlw.daria6918.cn

[Q47] 与平均值比较
来源：http://abc.bbcook.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://poe.meibo888.top

[Q48] CTE 公用表表达式
来源：http://nkg.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://frp.vqdsnc.cn

SELECT * FROM t WHERE c > 5;
来源：http://sds.tian-w.cn

[Q49] 更新单行
来源：http://nzd.fanxiaobao.xyz

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ohi.meibo888.top

[Q50] 批量更新
来源：http://ygh.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gwz.dashuyun.cn

[Q51] 用子查询更新
来源：http://rdh.xinyue.icu

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://fas.yueranfly.top

[Q52] 删除指定行
来源：http://bkv.jinyuanbaomall.cn

DELETE FROM users WHERE id = 10;
来源：http://bpg.nanxinkj.top

[Q53] 按条件删除
来源：http://csy.shanyushiyangtech.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jcr.feifeiyinyue.top

[Q54] 清空表
来源：http://mom.fzhhl.top

TRUNCATE TABLE logs;
来源：http://cso.shzxlz.cn

[Q55] 排名（并列占位）
来源：http://vrd.yj20258.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://njb.52xcode.cn

[Q56] 密集排名（并列不占位）
来源：http://gms.hywenlv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://gom.ywan-chungtsiang.top

[Q57] 行号
来源：http://yms.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://una.hywenlv.cn

[Q58] 累计求和
来源：http://zha.zhaomingkeji.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xpk.c1oappe.top

[Q59] 分组内累计
来源：http://eab.jyoumei.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yts.dashuyun.cn

[Q60] 取上一行 / 下一行
来源：http://yfe.fktsv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://fij.fzhhl.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wvv.hywenlv.cn

[Q61] 移动平均
来源：http://scu.hcnkem.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://buc.jinghuilouyu.cn

[Q62] 分组占比
来源：http://idk.xziqi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://fzn.sysykeji.top

[Q63] 开启事务
来源：http://ogz.tarul.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ril.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://sns.zdbjq.cn

COMMIT;
来源：http://zzb.hysaishi.cn

[Q65] 回滚事务
来源：http://mpp.aizwys.cn

ROLLBACK;
来源：http://nvv.wangshuangyany.cn

[Q66] 行锁查询
来源：http://uom.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bjo.gaohongyu789.top

[Q67] 设置隔离级别
来源：http://ola.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dsa.shuidangran.top

[Q68] 保存点
来源：http://yra.shanyushiyangtech.top

SAVEPOINT sp1;
来源：http://boq.tian-w.cn

ROLLBACK TO sp1;
来源：http://sjw.yj20258888.top

[Q69] 查看执行计划
来源：http://hil.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ysc.cucudq.cn

[Q70] 更新统计信息
来源：http://iom.meibo888.top

ANALYZE TABLE users;
来源：http://vjq.zhengqikj.top

[Q71] 查看建表语句
来源：http://cgb.tianlin.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nlq.ctjpmb.com

[Q72] 查看索引
来源：http://vld.zhiwuduotai.top

SHOW INDEX FROM users;
来源：http://kia.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://wxh.ppjwa.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vgx.shangyingyoupin.top

[Q74] 强制使用索引
来源：http://xll.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qwd.cqqwz.cn

[Q75] 日期格式化
来源：http://pxo.ywan-chungtsiang.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wpq.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://toy.tian-w.cn

[Q76] 按天统计
来源：http://ecl.zhaomingkeji.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ijg.yongpay.top

[Q77] 时间加减
来源：http://gsf.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://oyq.vqdsnc.cn

[Q78] 当前时间
来源：http://gtc.haohaochexian.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cxh.tarul.cn

[Q79] 字符串拼接
来源：http://jwq.nwbrower.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://glh.guowangkeji.top

[Q80] 字符串截取
来源：http://sik.zhiwuduotai.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bsr.fanxiaobao.xyz

[Q81] 字符串替换
来源：http://jnb.yongpay.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ewr.fanxiaobao.xyz

[Q82] 字符长度与字节长度
来源：http://ylr.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rcu.gaohongyu789.top

[Q83] 大小写转换
来源：http://jon.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://trj.xuanzx.com

[Q84] 去除首尾空格
来源：http://uge.zdqjudy.top

SELECT TRIM(name) FROM users;
来源：http://qlm.xuetiantiany.cn

[Q85] 数值取整
来源：http://pqm.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wos.yj20258888.top

[Q86] 读取 JSON 字段
来源：http://moz.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://diq.tianlin.xyz

[Q87] JSON 字段做条件
来源：http://axd.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://udu.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://tpx.fanxiaobao.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zga.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uwt.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://vkr.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rpz.gaohongyu789.top

[Q90] 生成序号列
来源：http://zef.tanke756.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://rwv.shanyushiyangtech.top

================================================================================
来源：http://kqu.dashuyun.cn

R. Bash 专题
来源：http://nsi.haohaochexian.top

================================================================================
来源：http://afz.xinyue.icu

[R01] shebang 与严格模式
来源：http://qtx.fehbvm.com

#!/usr/bin/env bash
来源：http://zwe.jinqigfzy.top

set -euo pipefail
来源：http://rrt.nwbrower.top

[R02] 变量赋值与使用
来源：http://bdp.52xcode.cn

name="Tom"; echo "$name"
来源：http://uhj.tarul.cn

[R03] 只读变量
来源：http://vkl.9152youxi.cn

readonly PI=3.14
来源：http://tly.ivvv.top

[R04] 位置参数
来源：http://wps.gotoacloud.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cpf.zhoulong.xyz

[R05] 参数默认值
来源：http://fdp.yfazqb.com

name="${1:-default}"
来源：http://hwl.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://ajn.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://clp.jianghu66.top

[R07] if 判断文件
来源：http://yuj.fanxiaobao.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://txt.kuanghao11.cn

[R08] 数值比较
来源：http://iap.316326.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://ihj.cheryme.top

[R09] 字符串比较
来源：http://lrk.dashuyun.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://skv.hfpthk.cn

[R10] 正则匹配
来源：http://ngo.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yze.dashuyun.cn

[R11] case 多分支
来源：http://pix.cashguo.top

case "$1" in
来源：http://ire.fktsv.cn

start) echo "启动" ;;
来源：http://uan.chenzaomai.com

stop)  echo "停止" ;;
来源：http://wqn.aizwys.cn

*)     echo "未知命令" ;;
来源：http://fmm.cqqwz.cn

esac
来源：http://zjj.316326.xyz

[R12] for 遍历文件
来源：http://vnw.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://iwr.mhx1999.top

[R13] for 计数循环
来源：http://vvb.nwbrower.top

for i in {1..10}; do echo "$i"; done
来源：http://ryh.daxiang520.top

[R14] C 风格 for
来源：http://sur.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cpf.hongshengwenyu.top

[R15] while 逐行读文件
来源：http://iqt.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://efb.gogol.net.cn

[R16] until 等待条件
来源：http://vai.xylfe.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xtn.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://trw.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://yhe.zhengqikj.top

[R18] 遍历数组
来源：http://jai.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hpp.52xcode.cn

[R19] 数组长度
来源：http://gga.redwolf501.top

echo "${#arr[@]}"
来源：http://ihd.vqdsnc.cn

[R20] 关联数组（字典）
来源：http://jes.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kuw.zhengqikj.top

[R21] 字符串长度
来源：http://ssx.smart0.xyz

echo "${#s}"
来源：http://wdm.vqdsnc.cn

[R22] 截取子串
来源：http://lrh.sufxvd.cn

echo "${s:0:5}"
来源：http://nyr.yuanzhike.top

[R23] 字符串替换
来源：http://oav.daria6918.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ycf.zhijiandao.cn

[R24] 大小写转换
来源：http://wqn.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://qlz.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://isu.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lwg.yanxiufei.cn

[R26] 命令替换
来源：http://wkn.birdmap.top

now=$(date +%F); echo "$now"
来源：http://eds.ydjk.org.cn

[R27] 算术展开
来源：http://hsj.jqgufenzy.top

echo $((1 + 2 * 3))
来源：http://uqy.shangyingyoupin.top

[R28] 浮点运算
来源：http://rig.vehdjk.com

echo "scale=2; 10/3" | bc
来源：http://rjr.xylfe.cn

[R29] 定义函数
来源：http://xpe.gzhubu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qnf.9152youxi.cn

[R30] 函数返回状态码
来源：http://utr.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://xae.jianghu66.top

[R31] 局部变量
来源：http://gzb.cheryme.top

f() { local x=1; echo "$x"; }
来源：http://oyi.shangyingyoupin.top

[R32] 参数个数校验
来源：http://tva.zycfv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sit.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://kcm.jiagoushi.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jjd.hnxiangtu.top

[R34] 退出时清理
来源：http://jtm.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vxf.xinyue.icu

[R35] 后台执行并等待
来源：http://jol.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://txp.cdnleiting.top

[R36] 并发执行多个任务
来源：http://nja.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uyv.yanxiufei.cn

[R37] 把输出赋给变量
来源：http://svw.gaohongyu789.top

files=$(ls -1)
来源：http://zrs.smart0.xyz

[R38] 管道串联
来源：http://ndu.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://yws.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://adu.kuanghao11.cn

cmd > out.log 2>&1
来源：http://syp.shzxlz.cn

[R40] 追加写日志
来源：http://pjy.snrcjt.cn

echo "log" >> out.log
来源：http://llp.tian-w.cn

[R41] 丢弃输出
来源：http://iat.ivvv.top

cmd >/dev/null 2>&1
来源：http://ovy.yj20258.top

[R42] 输入重定向
来源：http://hta.fanxiaobao.xyz

wc -l < a.txt
来源：http://osb.smart0.xyz

[R43] 按名字查找文件
来源：http://hmy.zdqjudy.top

find . -name "*.log" -type f
来源：http://bld.mhx1999.top

[R44] 按修改时间查找
来源：http://ulf.svipenyu.cn

find . -mtime -7 -type f
来源：http://ipi.fengsongda.top

[R45] 批量删除
来源：http://oeg.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://vre.fengsongda.top

[R46] 递归替换文件内容
来源：http://txf.sxryk.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lue.cdnleiting.top

[R47] sed 单行替换
来源：http://nqr.feifeiyinyue.top

sed -i 's/foo/bar/g' a.txt
来源：http://aoc.hnxiangtu.top

[R48] awk 取指定列
来源：http://jkw.chenjidiqi.icu

awk '{print $1, $3}' a.txt
来源：http://bgc.nanxuanxn.top

[R49] awk 带条件
来源：http://bks.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bze.ydjk.org.cn

[R50] awk 求和
来源：http://yel.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://icg.hcnkem.com

[R51] 排序去重取前几
来源：http://oww.wangdashe.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dbv.redwolf501.top

[R52] 统计行数
来源：http://wga.ctjpmb.com

wc -l a.txt
来源：http://nxk.yangfankeji.com

[R53] 查看文件头与实时尾
来源：http://bcf.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tre.nanxinkj.top

[R54] 比较两个文件
来源：http://nwr.zhiwuduotai.top

diff a.txt b.txt
来源：http://fyt.zhiwuduotai.top

[R55] 压缩与解压
来源：http://umd.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://thw.cashguo.top

[R56] 远程拷贝
来源：http://uny.ppjwa.cn

scp file user@host:/path/
来源：http://cvn.c1oappe.top

[R57] 远程执行命令
来源：http://lvg.ivvv.top

ssh user@host 'uptime'
来源：http://prs.bjfxy.top

[R58] 下载文件
来源：http://mjb.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ikw.gogol.net.cn

[R59] 发 POST JSON
来源：http://fdv.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://czq.yvedp.cn

[R60] 只看 HTTP 状态码
来源：http://qlt.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vqf.ivvv.top

[R61] 磁盘占用
来源：http://yzo.xuetiantiany.cn

df -h;  du -sh *
来源：http://znt.sxryk.cn

[R62] 找最占空间的文件
来源：http://jrt.dianchejie.cn

du -ah . | sort -rh | head -10
来源：http://ogx.andypj.xyz

[R63] 内存与进程
来源：http://lud.yonumen.top

free -h;  ps aux | grep nginx
来源：http://tsf.wangdashe.top

[R64] 结束进程
来源：http://pqm.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://fzn.ctjpmb.com

[R65] 查看端口占用
来源：http://hky.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://slr.zhixingplan.top

[R66] 定时任务
来源：http://mnf.iojbl.cn

crontab -e;  crontab -l
来源：http://kuu.daria6918.cn

[R67] 生成随机十六进制串
来源：http://gmc.chenjidiqi.icu

openssl rand -hex 16
来源：http://kki.hnqzz.top

[R68] 计算文件校验值
来源：http://vse.quarkkingdee.top

sha256sum a.txt;  md5sum a.txt
来源：http://ioe.sxryk.cn

[R69] 生成随机密码
来源：http://ywq.shzxlz.cn

head -c 16 /dev/urandom | base64
来源：http://gxh.zhongyouzk.top

[R70] 时间戳与互转
来源：http://brm.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://jpw.daxiang520.top

[R71] 日期格式化
来源：http://wtj.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mkr.chenlongwang.top

[R72] 等待端口就绪
来源：http://qtx.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://iji.svipenyu.cn

[R73] 分割大日志
来源：http://epl.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://qst.shanyushiyangtech.top

[R74] 批量重命名
来源：http://ybe.ydjk.org.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fjt.ehwqpu.com

[R75] 导出环境变量
来源：http://zfe.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://glt.hcnkem.com

[R76] 使用临时文件
来源：http://zni.daria6918.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://olv.cqqwz.cn

[R77] 读取用户输入
来源：http://hmr.jyoumei.cn

read -rp "请输入: " ans
来源：http://ehh.wangdashe.top

[R78] 交互式菜单
来源：http://jjb.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zqt.hfpthk.cn

[R79] 解析命令行选项
来源：http://xcd.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://txg.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://jpq.c1oappe.top

time ./run.sh
来源：http://dle.yongpay.top

================================================================================
来源：http://eem.yvedp.cn

S. C / C++ 专题
来源：http://imx.epnwcf.com

================================================================================
来源：http://hcf.yuanzhike.top

[S01] C：Hello World
来源：http://exf.ppjwa.cn

#include <stdio.h>
来源：http://llz.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tno.gaohongyu789.top

[S02] C：变量与格式化输出
来源：http://qcq.hysaishi.cn

int a = 10; printf("%d\n", a);
来源：http://bnu.guowangkeji.top

[S03] C：读入整数
来源：http://egh.zhoulong.xyz

int x; scanf("%d", &x);
来源：http://uef.pengpengdd.cyou

[S04] C：字符串复制
来源：http://eyz.yangfankeji.com

char dst[32]; strcpy(dst, "hi");
来源：http://tvj.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://qsk.kuanghao11.cn

strlen(s)
来源：http://irx.hammf.cn

[S06] C：字符串比较
来源：http://xct.chenlongwang.top

strcmp(a, b) == 0
来源：http://ftz.316326.xyz

[S07] C：数组遍历求和
来源：http://tud.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://osd.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://aha.316326.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://shy.yvedp.cn

[S09] C：结构体定义与初始化
来源：http://mmg.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bxt.fanxiaobao.xyz

[S10] C：指针与解引用
来源：http://lfu.ivvv.top

int *p = &a;  *p = 5;
来源：http://dnx.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://oum.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://ctl.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wry.xylfe.cn

fclose(f);
来源：http://fqd.zhiwuduotai.top

[S12] C：写文件
来源：http://zqs.chenzaomai.com


<!-- 参考信息 -->