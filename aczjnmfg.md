代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://stp.nanxuanxn.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hjt.jianghu66.top

[Q43] 标量子查询
来源：http://igs.yfazqb.com

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hdi.c1oappe.top

[Q44] IN 子查询
来源：http://ezh.jiagoushi.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://tuv.yanxiufei.cn

[Q45] EXISTS 判断存在
来源：http://klh.yanxiufei.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mkx.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://gdn.yanxiufei.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rkb.yuxming.cn

[Q47] 与平均值比较
来源：http://qeb.nanxuanxn.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://fng.sufxvd.cn

[Q48] CTE 公用表表达式
来源：http://nrc.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xmc.dianchejie.cn

SELECT * FROM t WHERE c > 5;
来源：http://rsx.tianlin.xyz

[Q49] 更新单行
来源：http://lwj.dianchejie.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uzv.aizwys.cn

[Q50] 批量更新
来源：http://pmy.tian-w.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://jvb.zhiwuduotai.top

[Q51] 用子查询更新
来源：http://vzh.pengpengdd.cyou

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://say.yj20258888.top

[Q52] 删除指定行
来源：http://jda.xuanzx.com

DELETE FROM users WHERE id = 10;
来源：http://fxc.cdnleiting.top

[Q53] 按条件删除
来源：http://dbo.tianlin.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://yuu.guannengcc.top

[Q54] 清空表
来源：http://gkw.vehdjk.com

TRUNCATE TABLE logs;
来源：http://yzz.andypj.xyz

[Q55] 排名（并列占位）
来源：http://lqg.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ngo.hcnkem.com

[Q56] 密集排名（并列不占位）
来源：http://oob.guowangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sxe.yuxming.cn

[Q57] 行号
来源：http://fad.cashguo.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://xvw.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://dzb.snrcjt.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fnn.zdbjq.cn

[Q59] 分组内累计
来源：http://flb.fehbvm.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://fbb.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://kmc.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://par.hywenlv.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bvy.guowangkeji.top

[Q61] 移动平均
来源：http://vsd.sufxvd.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zat.yj20258888.top

[Q62] 分组占比
来源：http://gio.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://syw.jlsjyb.cn

[Q63] 开启事务
来源：http://aev.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://tkh.chenjidiqi.icu

[Q64] 提交事务
来源：http://azl.zhiwuduotai.top

COMMIT;
来源：http://ocz.zhoulong.xyz

[Q65] 回滚事务
来源：http://hzz.xingfuxueyuan.xyz

ROLLBACK;
来源：http://eal.sxryk.cn

[Q66] 行锁查询
来源：http://zph.hesvh.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://kic.hammf.cn

[Q67] 设置隔离级别
来源：http://lof.zycfv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zym.shanyushiyangtech.top

[Q68] 保存点
来源：http://ijs.snrcjt.cn

SAVEPOINT sp1;
来源：http://vnv.xylfe.cn

ROLLBACK TO sp1;
来源：http://neh.daria6918.cn

[Q69] 查看执行计划
来源：http://kmr.zhaomingkeji.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://knx.zdqjudy.top

[Q70] 更新统计信息
来源：http://rom.fanxiaobao.xyz

ANALYZE TABLE users;
来源：http://trm.fehbvm.com

[Q71] 查看建表语句
来源：http://mxd.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://fsy.ctjpmb.com

[Q72] 查看索引
来源：http://tif.316326.xyz

SHOW INDEX FROM users;
来源：http://nqg.yonumen.top

[Q73] 查看表状态
来源：http://dkc.jiagoushi.top

SHOW TABLE STATUS LIKE 'users';
来源：http://llx.jiagoushi.top

[Q74] 强制使用索引
来源：http://zll.xingfuxueyuan.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ijt.yanxiufei.cn

[Q75] 日期格式化
来源：http://bpo.smart0.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://rqu.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://byv.cashguo.top

[Q76] 按天统计
来源：http://qzm.shanyushiyangtech.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vag.shanyushiyangtech.top

[Q77] 时间加减
来源：http://piu.birdmap.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iay.jinqigufen.top

[Q78] 当前时间
来源：http://zpq.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ycu.guowangkeji.top

[Q79] 字符串拼接
来源：http://loy.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://and.bbcook.cn

[Q80] 字符串截取
来源：http://vtv.yueranfly.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hvc.hammf.cn

[Q81] 字符串替换
来源：http://lnn.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hlo.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://vac.shangyingyoupin.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://djq.hysaishi.cn

[Q83] 大小写转换
来源：http://eri.dashuyun.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://grp.hywenlv.cn

[Q84] 去除首尾空格
来源：http://wkd.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://dew.chenjidiqi.icu

[Q85] 数值取整
来源：http://mfa.gaohongyu789.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gje.9152youxi.cn

[Q86] 读取 JSON 字段
来源：http://ynj.tarul.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rqg.316326.xyz

[Q87] JSON 字段做条件
来源：http://dbr.tanke756.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uit.c1oappe.top

[Q88] 行转列（条件聚合）
来源：http://vkb.zycfv.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fqt.yongpay.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dyu.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://iyn.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ccg.yongpay.top

[Q90] 生成序号列
来源：http://lhz.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zgi.meibo888.top

================================================================================
来源：http://ahm.nanxinkj.top

R. Bash 专题
来源：http://vkv.hammf.cn

================================================================================
来源：http://ezh.yonumen.top

[R01] shebang 与严格模式
来源：http://xvp.jqgufenzy.top

#!/usr/bin/env bash
来源：http://rnm.jqgufenzy.top

set -euo pipefail
来源：http://ouy.ydjk.org.cn

[R02] 变量赋值与使用
来源：http://wha.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://avv.hnqzz.top

[R03] 只读变量
来源：http://yhm.zycfv.cn

readonly PI=3.14
来源：http://szp.tian-w.cn

[R04] 位置参数
来源：http://fjn.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wso.mhx1999.top

[R05] 参数默认值
来源：http://flr.yj20258888.top

name="${1:-default}"
来源：http://ucy.ivvv.top

[R06] 判断命令是否存在
来源：http://fry.zdbjq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hvu.yonumen.top

[R07] if 判断文件
来源：http://nps.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jfs.zhiwuduotai.top

[R08] 数值比较
来源：http://nbe.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ids.shangyingyoupin.top

[R09] 字符串比较
来源：http://egh.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvf.yuanzhike.top

[R10] 正则匹配
来源：http://hau.shanyushiyangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zdw.hesvh.cn

[R11] case 多分支
来源：http://nwi.jinqigufen.top

case "$1" in
来源：http://nyq.tian-w.cn

start) echo "启动" ;;
来源：http://dsg.tian-w.cn

stop)  echo "停止" ;;
来源：http://lsb.52xcode.cn

*)     echo "未知命令" ;;
来源：http://cmm.shuidangran.top

esac
来源：http://kpb.havefunace.top

[R12] for 遍历文件
来源：http://cvt.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://whe.nanxuanxn.top

[R13] for 计数循环
来源：http://mds.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://xgi.ctjpmb.com

[R14] C 风格 for
来源：http://krr.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ewe.c1oappe.top

[R15] while 逐行读文件
来源：http://uwj.vqdsnc.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lck.wangdashe.top

[R16] until 等待条件
来源：http://yuk.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qev.tianlin.xyz

[R17] 数组定义与取值
来源：http://sat.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://akq.hcnkem.com

[R18] 遍历数组
来源：http://akh.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cpz.gogol.net.cn

[R19] 数组长度
来源：http://xai.pengpengdd.cyou

echo "${#arr[@]}"
来源：http://ljj.wangdashe.top

[R20] 关联数组（字典）
来源：http://uxa.xziqi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://iuc.redwolf501.top

[R21] 字符串长度
来源：http://khn.hcnkem.com

echo "${#s}"
来源：http://nue.zhiwuduotai.top

[R22] 截取子串
来源：http://hki.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://nyh.cucudq.cn

[R23] 字符串替换
来源：http://anv.cucudq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bmm.wangdashe.top

[R24] 大小写转换
来源：http://jvp.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://qaq.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://wnd.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ouh.cucudq.cn

[R26] 命令替换
来源：http://vgx.yj20258.top

now=$(date +%F); echo "$now"
来源：http://hek.shanyushiyangtech.top

[R27] 算术展开
来源：http://cqu.cucudq.cn

echo $((1 + 2 * 3))
来源：http://kwj.zycfv.cn

[R28] 浮点运算
来源：http://erw.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://eun.hesvh.cn

[R29] 定义函数
来源：http://deq.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kmy.sysykeji.top

[R30] 函数返回状态码
来源：http://zod.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://lex.zycfv.cn

[R31] 局部变量
来源：http://zwo.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://xzu.zhoulong.xyz

[R32] 参数个数校验
来源：http://ggr.sweek.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kvt.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://oyo.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tws.guannengcc.top

[R34] 退出时清理
来源：http://hfe.yfazqb.com

trap 'rm -f "$tmp"' EXIT
来源：http://aet.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://hkp.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://gkp.jianghu66.top

[R36] 并发执行多个任务
来源：http://etk.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hrl.xziqi.cn

[R37] 把输出赋给变量
来源：http://kzw.gogol.net.cn

files=$(ls -1)
来源：http://cgh.gotoacloud.top

[R38] 管道串联
来源：http://dny.sweek.top

cat a.txt | grep -i error | wc -l
来源：http://xwg.uphjek.com

[R39] 重定向标准输出与错误
来源：http://ztu.zdqjudy.top

cmd > out.log 2>&1
来源：http://vyz.cashguo.top

[R40] 追加写日志
来源：http://yed.nanxuanxn.top

echo "log" >> out.log
来源：http://fcw.shanyushiyangtech.top

[R41] 丢弃输出
来源：http://jva.iojbl.cn

cmd >/dev/null 2>&1
来源：http://vok.bjfxy.top

[R42] 输入重定向
来源：http://zdj.zhongyouzk.top

wc -l < a.txt
来源：http://zlz.cashguo.top

[R43] 按名字查找文件
来源：http://kdy.chenlongwang.top

find . -name "*.log" -type f
来源：http://med.iojbl.cn

[R44] 按修改时间查找
来源：http://vxh.hcnkem.com

find . -mtime -7 -type f
来源：http://ddv.vqdsnc.cn

[R45] 批量删除
来源：http://naj.wangdashe.top

find . -name "*.tmp" -delete
来源：http://fon.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://yfj.cdnleiting.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hzr.yangfankeji.com

[R47] sed 单行替换
来源：http://rhj.cashguo.top

sed -i 's/foo/bar/g' a.txt
来源：http://dgz.bbcook.cn

[R48] awk 取指定列
来源：http://ure.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://yqg.hammf.cn

[R49] awk 带条件
来源：http://aib.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gxn.chenzaomai.com

[R50] awk 求和
来源：http://wjn.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://xum.yanxiufei.cn

[R51] 排序去重取前几
来源：http://mgi.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://dls.quarkkingdee.top

[R52] 统计行数
来源：http://kkm.chenjidiqi.icu

wc -l a.txt
来源：http://esl.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://hax.wangdashe.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tvt.ppjwa.cn

[R54] 比较两个文件
来源：http://xse.fzhhl.top

diff a.txt b.txt
来源：http://oau.feifeiyinyue.top

[R55] 压缩与解压
来源：http://fwf.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oda.gaohongyu789.top

[R56] 远程拷贝
来源：http://xga.sjlbkw.cn

scp file user@host:/path/
来源：http://pul.ppjwa.cn

[R57] 远程执行命令
来源：http://xww.zdbjq.cn

ssh user@host 'uptime'
来源：http://mkv.hammf.cn

[R58] 下载文件
来源：http://bfq.ehwqpu.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ikc.dashuyun.cn

[R59] 发 POST JSON
来源：http://qzr.yvedp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hln.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://xbd.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ktn.tian-w.cn

[R61] 磁盘占用
来源：http://sbe.jinghuilouyu.cn

df -h;  du -sh *
来源：http://mgf.uphjek.com

[R62] 找最占空间的文件
来源：http://awx.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://jkz.yj20258.top

[R63] 内存与进程
来源：http://zyc.ehwqpu.com

free -h;  ps aux | grep nginx
来源：http://knd.shanyushiyangkeji.top

[R64] 结束进程
来源：http://sgf.vqdsnc.cn

kill -9 $(pgrep -f app.py)
来源：http://pcf.hywenlv.cn

[R65] 查看端口占用
来源：http://lwn.shuidangran.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hpv.chenjidiqi.icu

[R66] 定时任务
来源：http://skh.aizwys.cn

crontab -e;  crontab -l
来源：http://lyd.tian-w.cn

[R67] 生成随机十六进制串
来源：http://njc.ctjpmb.com

openssl rand -hex 16
来源：http://zhm.wangdashe.top

[R68] 计算文件校验值
来源：http://ysa.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://sps.dianchejie.cn

[R69] 生成随机密码
来源：http://xur.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://fvk.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://dkq.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://gtw.svipenyu.cn

[R71] 日期格式化
来源：http://ifr.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gkd.aibaodan.cn

[R72] 等待端口就绪
来源：http://rdt.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://axs.guowangkeji.top

[R73] 分割大日志
来源：http://kzn.ppjwa.cn

split -l 1000 big.log part_
来源：http://fxt.hesvh.cn

[R74] 批量重命名
来源：http://nvc.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qqq.birdmap.top

[R75] 导出环境变量
来源：http://zlr.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://snz.xziqi.cn

[R76] 使用临时文件
来源：http://hub.feifeiyinyue.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ckm.tarul.cn

[R77] 读取用户输入
来源：http://hqr.wangdashe.top

read -rp "请输入: " ans
来源：http://qay.xingfuxueyuan.xyz

[R78] 交互式菜单
来源：http://has.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://pal.fktsv.cn

[R79] 解析命令行选项
来源：http://xdw.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ywe.mhx1999.top

[R80] 查看脚本执行耗时
来源：http://yye.sweek.top

time ./run.sh
来源：http://ovl.c1oappe.top

================================================================================
来源：http://bpa.chenlongwang.top

S. C / C++ 专题
来源：http://fwm.tarul.cn

================================================================================
来源：http://hjo.jqgufenzy.top

[S01] C：Hello World
来源：http://ixz.smart0.xyz

#include <stdio.h>
来源：http://mzd.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://vht.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://evg.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://kuy.epnwcf.com

[S03] C：读入整数
来源：http://pty.yj20258.top

int x; scanf("%d", &x);
来源：http://awd.yongpay.top

[S04] C：字符串复制
来源：http://oly.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://quk.xuanzx.com

[S05] C：字符串长度
来源：http://lfs.xylfe.cn

strlen(s)
来源：http://zgm.yongpay.top

[S06] C：字符串比较
来源：http://zng.wangshuangyany.cn

strcmp(a, b) == 0
来源：http://exq.nwbrower.top

[S07] C：数组遍历求和
来源：http://zrl.jqgfzy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qwj.uphjek.com

[S08] C：动态内存分配与释放
来源：http://gtw.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://olu.yj20258.top

[S09] C：结构体定义与初始化
来源：http://erx.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vbi.gzhubu.top

[S10] C：指针与解引用
来源：http://zsz.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://qka.havefunace.top

[S11] C：逐行读文件
来源：http://hid.0kj1m.cn

FILE *f = fopen("a.txt", "r");
来源：http://ohr.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pcq.nwbrower.top

fclose(f);
来源：http://mmz.iojbl.cn

[S12] C：写文件
来源：http://zlt.sjlbkw.cn


<!-- 参考信息 -->