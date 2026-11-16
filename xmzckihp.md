代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://qdj.xziqi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://rfw.dianchejie.cn

[Q47] 与平均值比较
来源：http://dfn.vqdsnc.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://efn.yangfankeji.com

[Q48] CTE 公用表表达式
来源：http://nrh.zdbjq.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://myv.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://enh.hysaishi.cn

[Q49] 更新单行
来源：http://svg.hnxiangtu.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://irw.tanke756.top

[Q50] 批量更新
来源：http://agu.shanyushiyangtech.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eio.fehbvm.com

[Q51] 用子查询更新
来源：http://jhb.xuanzx.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://zmw.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://gvy.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://ead.yangfankeji.com

[Q53] 按条件删除
来源：http://emp.andypj.xyz

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sel.pengpengdd.cyou

[Q54] 清空表
来源：http://oib.pycfn.com

TRUNCATE TABLE logs;
来源：http://mzv.havefunace.top

[Q55] 排名（并列占位）
来源：http://rxu.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fkr.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://cjr.cashguo.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nql.shanyushiyangtech.top

[Q57] 行号
来源：http://vwp.gotoacloud.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kqt.ywan-chungtsiang.top

[Q58] 累计求和
来源：http://hza.nwbrower.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fpq.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://ihl.sjlbkw.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kov.redwolf501.top

[Q60] 取上一行 / 下一行
来源：http://cck.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dzc.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ihi.jqgfzy.top

[Q61] 移动平均
来源：http://ovr.tanke756.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wtr.kuanghao11.cn

[Q62] 分组占比
来源：http://xlx.xuanzx.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lju.guannengcc.top

[Q63] 开启事务
来源：http://mjg.yanxiufei.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kpi.0kj1m.cn

[Q64] 提交事务
来源：http://szj.ppjwa.cn

COMMIT;
来源：http://xfx.c1oappe.top

[Q65] 回滚事务
来源：http://tcu.yvedp.cn

ROLLBACK;
来源：http://uih.zycfv.cn

[Q66] 行锁查询
来源：http://uxs.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jng.cdnleiting.top

[Q67] 设置隔离级别
来源：http://euz.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://gzq.pycfn.com

[Q68] 保存点
来源：http://fxo.yonumen.top

SAVEPOINT sp1;
来源：http://bux.xinyue.icu

ROLLBACK TO sp1;
来源：http://nzk.uphjek.com

[Q69] 查看执行计划
来源：http://tjd.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tka.cashguo.top

[Q70] 更新统计信息
来源：http://nih.yonumen.top

ANALYZE TABLE users;
来源：http://opd.nanxuanxn.top

[Q71] 查看建表语句
来源：http://mtf.wangdashe.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uhf.zhongyouzk.top

[Q72] 查看索引
来源：http://vge.guowangkeji.top

SHOW INDEX FROM users;
来源：http://jxd.ydjk.org.cn

[Q73] 查看表状态
来源：http://jav.nanxuanxn.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iov.daria6918.cn

[Q74] 强制使用索引
来源：http://gem.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://oeo.shangyingyoupin.top

[Q75] 日期格式化
来源：http://ubv.xuetiantiany.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ueh.mhx1999.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://bgq.hesvh.cn

[Q76] 按天统计
来源：http://mdz.haohaochexian.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://rmt.hcnkem.com

[Q77] 时间加减
来源：http://cra.wangshuangyany.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://byi.bbcook.cn

[Q78] 当前时间
来源：http://mzo.pycfn.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gum.jyoumei.cn

[Q79] 字符串拼接
来源：http://dwm.yangfankeji.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://loj.dianchejie.cn

[Q80] 字符串截取
来源：http://hmg.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tzq.sxryk.cn

[Q81] 字符串替换
来源：http://pyg.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://lul.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://nbm.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tgq.wangdashe.top

[Q83] 大小写转换
来源：http://jso.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://zrp.wangdashe.top

[Q84] 去除首尾空格
来源：http://gpc.chenzaomai.com

SELECT TRIM(name) FROM users;
来源：http://avm.bjfxy.top

[Q85] 数值取整
来源：http://wom.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bym.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://syx.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://imq.hongshengwenyu.top

[Q87] JSON 字段做条件
来源：http://eqa.svipenyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://dkq.zhiwuduotai.top

[Q88] 行转列（条件聚合）
来源：http://tnt.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hzn.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ccb.yonumen.top

[Q89] 判断表是否存在
来源：http://iaf.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pkv.sysykeji.top

[Q90] 生成序号列
来源：http://mfh.yvedp.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vau.hnqzz.top

================================================================================
来源：http://ane.hywenlv.cn

R. Bash 专题
来源：http://juq.ydjk.org.cn

================================================================================
来源：http://cdc.chenlongwang.top

[R01] shebang 与严格模式
来源：http://rfq.dashuyun.cn

#!/usr/bin/env bash
来源：http://oks.daria6918.cn

set -euo pipefail
来源：http://jnr.yuxming.cn

[R02] 变量赋值与使用
来源：http://sml.snrcjt.cn

name="Tom"; echo "$name"
来源：http://tie.ctjpmb.com

[R03] 只读变量
来源：http://ump.ppjwa.cn

readonly PI=3.14
来源：http://cqn.jinyuanbaomall.cn

[R04] 位置参数
来源：http://pcz.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://puo.snrcjt.cn

[R05] 参数默认值
来源：http://vba.yangfankeji.com

name="${1:-default}"
来源：http://ryt.52xcode.cn

[R06] 判断命令是否存在
来源：http://hgb.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pnx.birdmap.top

[R07] if 判断文件
来源：http://onw.chenlongwang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pug.fanxiaobao.xyz

[R08] 数值比较
来源：http://hkb.hnqzz.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sic.yj202588.top

[R09] 字符串比较
来源：http://doq.fengsongda.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gir.sysykeji.top

[R10] 正则匹配
来源：http://fxc.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ipu.pycfn.com

[R11] case 多分支
来源：http://ilf.hnxiangtu.top

case "$1" in
来源：http://oyc.gzhubu.top

start) echo "启动" ;;
来源：http://ixa.shuidangran.top

stop)  echo "停止" ;;
来源：http://mte.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://ftj.vehdjk.com

esac
来源：http://zce.jyoumei.cn

[R12] for 遍历文件
来源：http://vns.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://ykn.9152youxi.cn

[R13] for 计数循环
来源：http://hfm.xinyue.icu

for i in {1..10}; do echo "$i"; done
来源：http://bjt.tarul.cn

[R14] C 风格 for
来源：http://zgk.aibaodan.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qkv.kuanghao11.cn

[R15] while 逐行读文件
来源：http://enp.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rih.hcnkem.com

[R16] until 等待条件
来源：http://blh.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rrz.meibo888.top

[R17] 数组定义与取值
来源：http://njk.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://pbt.hesvh.cn

[R18] 遍历数组
来源：http://ynq.gotoacloud.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gtb.0kj1m.cn

[R19] 数组长度
来源：http://rlt.fzhhl.top

echo "${#arr[@]}"
来源：http://nxy.fehbvm.com

[R20] 关联数组（字典）
来源：http://nor.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://csd.hnqzz.top

[R21] 字符串长度
来源：http://rzr.nanxuanxn.top

echo "${#s}"
来源：http://wgg.ydzc1.top

[R22] 截取子串
来源：http://yhw.hywenlv.cn

echo "${s:0:5}"
来源：http://tvs.sufxvd.cn

[R23] 字符串替换
来源：http://mlh.gaohongyu789.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xpz.chenzaomai.com

[R24] 大小写转换
来源：http://uda.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://qhi.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://esj.sufxvd.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://upe.zhongyouzk.top

[R26] 命令替换
来源：http://ptz.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://dzo.xuanzx.com

[R27] 算术展开
来源：http://ezt.mhx1999.top

echo $((1 + 2 * 3))
来源：http://kwc.xingfuxueyuan.xyz

[R28] 浮点运算
来源：http://vmp.ctjpmb.com

echo "scale=2; 10/3" | bc
来源：http://rwk.52xcode.cn

[R29] 定义函数
来源：http://ysv.smart0.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bdh.yongpay.top

[R30] 函数返回状态码
来源：http://smk.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://hmy.yuxming.cn

[R31] 局部变量
来源：http://otj.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://ghb.tianlin.xyz

[R32] 参数个数校验
来源：http://nlv.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hyz.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://oyb.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://veh.meibo888.top

[R34] 退出时清理
来源：http://ios.hnxiangtu.top

trap 'rm -f "$tmp"' EXIT
来源：http://sih.havefunace.top

[R35] 后台执行并等待
来源：http://hjw.yj20258888.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dqj.xylfe.cn

[R36] 并发执行多个任务
来源：http://ihu.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zfj.guannengcc.top

[R37] 把输出赋给变量
来源：http://ttp.kuanghao11.cn

files=$(ls -1)
来源：http://wbx.xingfuxueyuan.xyz

[R38] 管道串联
来源：http://rmi.zdqjudy.top

cat a.txt | grep -i error | wc -l
来源：http://iuo.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://asn.xingfuxueyuan.xyz

cmd > out.log 2>&1
来源：http://dbr.hcnkem.com

[R40] 追加写日志
来源：http://qrz.jinghuilouyu.cn

echo "log" >> out.log
来源：http://wuo.daxiang520.top

[R41] 丢弃输出
来源：http://xps.tanke756.top

cmd >/dev/null 2>&1
来源：http://bjx.zdqjudy.top

[R42] 输入重定向
来源：http://sbw.jinqigufen.top

wc -l < a.txt
来源：http://wbi.epnwcf.com

[R43] 按名字查找文件
来源：http://toy.jyoumei.cn

find . -name "*.log" -type f
来源：http://fru.shangyingyoupin.top

[R44] 按修改时间查找
来源：http://cxx.yangfankeji.com

find . -mtime -7 -type f
来源：http://jpu.ydzc1.top

[R45] 批量删除
来源：http://hjz.daxiang520.top

find . -name "*.tmp" -delete
来源：http://fmq.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://dye.wangshuangyany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gns.zhiwuduotai.top

[R47] sed 单行替换
来源：http://xzk.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://beg.fzhhl.top

[R48] awk 取指定列
来源：http://mpo.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://mbh.jianghu66.top

[R49] awk 带条件
来源：http://wza.ehwqpu.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iql.jlsjyb.cn

[R50] awk 求和
来源：http://kbm.9152youxi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://irc.jinyuanbaomall.cn

[R51] 排序去重取前几
来源：http://afm.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://lvh.yfazqb.com

[R52] 统计行数
来源：http://ouw.hongshengwenyu.top

wc -l a.txt
来源：http://mcd.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://kgm.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://aqi.shangyingyoupin.top

[R54] 比较两个文件
来源：http://dzo.snrcjt.cn

diff a.txt b.txt
来源：http://ofv.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://kpm.shuidangran.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://pfi.ppjwa.cn

[R56] 远程拷贝
来源：http://bin.hysaishi.cn

scp file user@host:/path/
来源：http://laz.sysykeji.top

[R57] 远程执行命令
来源：http://gjf.zhengqikj.top

ssh user@host 'uptime'
来源：http://sxy.shzxlz.cn

[R58] 下载文件
来源：http://aqr.yangfankeji.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rsr.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://erl.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tdg.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://ech.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eow.sxryk.cn

[R61] 磁盘占用
来源：http://ihf.yonumen.top

df -h;  du -sh *
来源：http://wun.dashuyun.cn

[R62] 找最占空间的文件
来源：http://mep.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://myr.52xcode.cn

[R63] 内存与进程
来源：http://tdy.jinqigufen.top

free -h;  ps aux | grep nginx
来源：http://boz.hywenlv.cn

[R64] 结束进程
来源：http://kmn.chenjidiqi.icu

kill -9 $(pgrep -f app.py)
来源：http://uaf.nanxinkj.top

[R65] 查看端口占用
来源：http://ibm.iojbl.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://asp.zhoulong.xyz

[R66] 定时任务
来源：http://yvv.dianchejie.cn

crontab -e;  crontab -l
来源：http://kec.ydzc1.top

[R67] 生成随机十六进制串
来源：http://dyl.yueranfly.top

openssl rand -hex 16
来源：http://ncr.nanxuanxn.top

[R68] 计算文件校验值
来源：http://enz.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://fky.jlsjyb.cn

[R69] 生成随机密码
来源：http://kqv.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://kfj.wangdashe.top

[R70] 时间戳与互转
来源：http://rxx.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://epl.yonumen.top

[R71] 日期格式化
来源：http://bhh.sweek.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vpu.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://fjp.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nbq.zhiwuduotai.top

[R73] 分割大日志
来源：http://sqm.hnxiangtu.top

split -l 1000 big.log part_
来源：http://vfe.zhijiandao.cn

[R74] 批量重命名
来源：http://vkl.guowangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cih.zhaomingkeji.xyz

[R75] 导出环境变量
来源：http://qzb.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://zcl.cdnleiting.top

[R76] 使用临时文件
来源：http://hnm.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://edc.epnwcf.com

[R77] 读取用户输入
来源：http://kef.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://lab.yj20258888.top

[R78] 交互式菜单
来源：http://cko.c1oappe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qjp.hysaishi.cn

[R79] 解析命令行选项
来源：http://avm.0kj1m.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vyr.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://knf.yonumen.top

time ./run.sh
来源：http://hvw.chenzaomai.com

================================================================================
来源：http://qyu.yuanzhike.top

S. C / C++ 专题
来源：http://pfn.meibo888.top

================================================================================
来源：http://kqs.yueranfly.top

[S01] C：Hello World
来源：http://bdq.redwolf501.top

#include <stdio.h>
来源：http://nus.chenlongwang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jsr.xuanzx.com

[S02] C：变量与格式化输出
来源：http://usr.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://qtc.xylfe.cn

[S03] C：读入整数
来源：http://eir.havefunace.top

int x; scanf("%d", &x);
来源：http://jsb.aizwys.cn

[S04] C：字符串复制
来源：http://vtz.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://hix.c1oappe.top

[S05] C：字符串长度
来源：http://afh.quarkkingdee.top

strlen(s)
来源：http://llh.andypj.xyz

[S06] C：字符串比较
来源：http://spq.aibaodan.cn

strcmp(a, b) == 0
来源：http://rnd.havefunace.top

[S07] C：数组遍历求和
来源：http://pgx.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rot.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://esp.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hcg.redwolf501.top

[S09] C：结构体定义与初始化
来源：http://xnw.epnwcf.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mfe.yanxiufei.cn

[S10] C：指针与解引用
来源：http://laz.bjfxy.top

int *p = &a;  *p = 5;
来源：http://iyx.zycfv.cn

[S11] C：逐行读文件
来源：http://euo.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://kww.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tbp.ivvv.top

fclose(f);
来源：http://hdi.zhiwuduotai.top

[S12] C：写文件
来源：http://lfi.tianlin.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zub.jlsjyb.cn

[S13] C：宏定义
来源：http://jks.yueranfly.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uax.jinghuilouyu.cn

[S14] C：枚举
来源：http://ykl.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://wtq.yj20258888.top

[S15] C：类型转换
来源：http://tbq.aibaodan.cn

(double) a / b
来源：http://fyb.yuanzhike.top

[S16] C：位操作置位
来源：http://yew.hesvh.cn


<!-- 参考信息 -->