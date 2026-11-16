代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://pny.chenlongwang.top

[Q50] 批量更新
来源：http://kvr.chenlongwang.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zkw.daxiang520.top

[Q51] 用子查询更新
来源：http://xor.jqgfzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ghk.epnwcf.com

[Q52] 删除指定行
来源：http://vko.cdnleiting.top

DELETE FROM users WHERE id = 10;
来源：http://xkp.yongpay.top

[Q53] 按条件删除
来源：http://vtq.jinyuanbaomall.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hgg.tarul.cn

[Q54] 清空表
来源：http://wuc.shanyushiyangkeji.top

TRUNCATE TABLE logs;
来源：http://pco.shuidangran.top

[Q55] 排名（并列占位）
来源：http://maf.snrcjt.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ijd.hfpthk.cn

[Q56] 密集排名（并列不占位）
来源：http://fwf.hammf.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://huu.yanxiufei.cn

[Q57] 行号
来源：http://aog.epnwcf.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ptf.jlsjyb.cn

[Q58] 累计求和
来源：http://nhn.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://esd.feifeiyinyue.top

[Q59] 分组内累计
来源：http://obr.jqgfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dnl.jqgufenzy.top

[Q60] 取上一行 / 下一行
来源：http://shl.sjlbkw.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ajn.9152youxi.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uvm.yfazqb.com

[Q61] 移动平均
来源：http://yam.shuidangran.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://knn.xingfuxueyuan.xyz

[Q62] 分组占比
来源：http://hqy.hcnkem.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lbi.hnqzz.top

[Q63] 开启事务
来源：http://wmf.ywan-chungtsiang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://edh.hywenlv.cn

[Q64] 提交事务
来源：http://nyc.nanxuanxn.top

COMMIT;
来源：http://cbd.yongpay.top

[Q65] 回滚事务
来源：http://afs.sweek.top

ROLLBACK;
来源：http://kqz.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://trh.zycfv.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qop.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://jtq.fehbvm.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://afq.cashguo.top

[Q68] 保存点
来源：http://ofm.ehwqpu.com

SAVEPOINT sp1;
来源：http://vya.svipenyu.cn

ROLLBACK TO sp1;
来源：http://xwf.nwbrower.top

[Q69] 查看执行计划
来源：http://qju.aibaodan.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rsh.aizwys.cn

[Q70] 更新统计信息
来源：http://ral.daria6918.cn

ANALYZE TABLE users;
来源：http://xjn.316326.xyz

[Q71] 查看建表语句
来源：http://isk.hammf.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://unv.nwbrower.top

[Q72] 查看索引
来源：http://xie.shzxlz.cn

SHOW INDEX FROM users;
来源：http://eyx.dianchejie.cn

[Q73] 查看表状态
来源：http://aoc.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://wrq.yj202588.top

[Q74] 强制使用索引
来源：http://yiv.daria6918.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://srv.zdqjudy.top

[Q75] 日期格式化
来源：http://lig.daxiang520.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qgc.epnwcf.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vta.hnxiangtu.top

[Q76] 按天统计
来源：http://hou.yanxiufei.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vyp.svipenyu.cn

[Q77] 时间加减
来源：http://qyq.snrcjt.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://onb.hysaishi.cn

[Q78] 当前时间
来源：http://amm.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://svz.xinyue.icu

[Q79] 字符串拼接
来源：http://cnw.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://shg.sjlbkw.cn

[Q80] 字符串截取
来源：http://rff.tianlin.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dgn.meibo888.top

[Q81] 字符串替换
来源：http://gnr.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jos.iojbl.cn

[Q82] 字符长度与字节长度
来源：http://biu.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kyu.ivvv.top

[Q83] 大小写转换
来源：http://xrp.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wlq.smart0.xyz

[Q84] 去除首尾空格
来源：http://nku.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://xmi.aibaodan.cn

[Q85] 数值取整
来源：http://qnc.mhx1999.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tgv.feifeiyinyue.top

[Q86] 读取 JSON 字段
来源：http://dnm.hesvh.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kau.cheryme.top

[Q87] JSON 字段做条件
来源：http://iam.pycfn.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fsn.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://fil.hnqzz.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jwu.ydzc1.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qpm.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://uin.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kcr.nanxinkj.top

[Q90] 生成序号列
来源：http://uxa.jinyuanbaomall.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmr.shzxlz.cn

================================================================================
来源：http://jjw.svipenyu.cn

R. Bash 专题
来源：http://qys.yvedp.cn

================================================================================
来源：http://ioi.pycfn.com

[R01] shebang 与严格模式
来源：http://uen.jqgufenzy.top

#!/usr/bin/env bash
来源：http://lor.ivvv.top

set -euo pipefail
来源：http://kos.sweek.top

[R02] 变量赋值与使用
来源：http://ozn.jyoumei.cn

name="Tom"; echo "$name"
来源：http://uff.zhixingplan.top

[R03] 只读变量
来源：http://mdg.vqdsnc.cn

readonly PI=3.14
来源：http://hzz.wangdashe.top

[R04] 位置参数
来源：http://szh.yueranfly.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wqr.tanke756.top

[R05] 参数默认值
来源：http://faq.havefunace.top

name="${1:-default}"
来源：http://nvf.bbcook.cn

[R06] 判断命令是否存在
来源：http://ofj.sjlbkw.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xdm.zhaomingkeji.xyz

[R07] if 判断文件
来源：http://slb.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ndv.aizwys.cn

[R08] 数值比较
来源：http://ojp.tanke756.top

if (( a > b )); then echo "a 更大"; fi
来源：http://asj.chenzaomai.com

[R09] 字符串比较
来源：http://bov.316326.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xnl.chenzaomai.com

[R10] 正则匹配
来源：http://jvo.smart0.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zyf.0kj1m.cn

[R11] case 多分支
来源：http://cfe.andypj.xyz

case "$1" in
来源：http://gns.yongpay.top

start) echo "启动" ;;
来源：http://okr.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://jwy.shanyushiyangkeji.top

*)     echo "未知命令" ;;
来源：http://ish.jinqigfzy.top

esac
来源：http://owy.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://pii.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://vgo.havefunace.top

[R13] for 计数循环
来源：http://jaw.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://cvm.quarkkingdee.top

[R14] C 风格 for
来源：http://bpz.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sgd.pycfn.com

[R15] while 逐行读文件
来源：http://qul.birdmap.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hjk.dianchejie.cn

[R16] until 等待条件
来源：http://lem.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eoj.bjfxy.top

[R17] 数组定义与取值
来源：http://ubw.fengsongda.top

arr=(a b c); echo "${arr[0]}"
来源：http://mwq.epnwcf.com

[R18] 遍历数组
来源：http://jgj.wangdashe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://akb.sxryk.cn

[R19] 数组长度
来源：http://vkt.guannengcc.top

echo "${#arr[@]}"
来源：http://say.fzhhl.top

[R20] 关联数组（字典）
来源：http://xos.sufxvd.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dje.sysykeji.top

[R21] 字符串长度
来源：http://avo.haohaochexian.top

echo "${#s}"
来源：http://mlw.yj20258.top

[R22] 截取子串
来源：http://cdl.cdnleiting.top

echo "${s:0:5}"
来源：http://dhg.yj20258888.top

[R23] 字符串替换
来源：http://kzj.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hjp.pengpengdd.cyou

[R24] 大小写转换
来源：http://jhc.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://oba.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://dda.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sml.chenlongwang.top

[R26] 命令替换
来源：http://spk.kuanghao11.cn

now=$(date +%F); echo "$now"
来源：http://cay.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://ewo.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://jcd.pengpengdd.cyou

[R28] 浮点运算
来源：http://fqp.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://twy.bbcook.cn

[R29] 定义函数
来源：http://qpc.jinyuanbaomall.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uqo.zhixingplan.top

[R30] 函数返回状态码
来源：http://qru.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://ymy.ydzc1.top

[R31] 局部变量
来源：http://lct.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://eua.xuanzx.com

[R32] 参数个数校验
来源：http://vfe.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://izh.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://goy.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xks.zhoulong.xyz

[R34] 退出时清理
来源：http://tuy.shuidangran.top

trap 'rm -f "$tmp"' EXIT
来源：http://sqj.fengsongda.top

[R35] 后台执行并等待
来源：http://wgo.xuanzx.com

sleep 5 & pid=$!; wait "$pid"
来源：http://xjk.cucudq.cn

[R36] 并发执行多个任务
来源：http://ukj.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gof.quarkkingdee.top

[R37] 把输出赋给变量
来源：http://fsr.yj20258888.top

files=$(ls -1)
来源：http://pzm.pycfn.com

[R38] 管道串联
来源：http://tbm.guowangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://qwp.tianlin.xyz

[R39] 重定向标准输出与错误
来源：http://hfg.meibo888.top

cmd > out.log 2>&1
来源：http://vwj.ctjpmb.com

[R40] 追加写日志
来源：http://wnt.fktsv.cn

echo "log" >> out.log
来源：http://znw.zhijiandao.cn

[R41] 丢弃输出
来源：http://nhc.feifeiyinyue.top

cmd >/dev/null 2>&1
来源：http://mdh.cheryme.top

[R42] 输入重定向
来源：http://tvw.hfpthk.cn

wc -l < a.txt
来源：http://ogy.fehbvm.com

[R43] 按名字查找文件
来源：http://wmm.sysykeji.top

find . -name "*.log" -type f
来源：http://qec.chenlongwang.top

[R44] 按修改时间查找
来源：http://shm.aibaodan.cn

find . -mtime -7 -type f
来源：http://oxp.jinghuilouyu.cn

[R45] 批量删除
来源：http://xpk.vehdjk.com

find . -name "*.tmp" -delete
来源：http://qwi.wangdashe.top

[R46] 递归替换文件内容
来源：http://jiu.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hcs.cheryme.top

[R47] sed 单行替换
来源：http://qut.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dgm.tarul.cn

[R48] awk 取指定列
来源：http://qmr.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://pqi.tianlin.xyz

[R49] awk 带条件
来源：http://ake.shangyingyoupin.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://olc.kuanghao11.cn

[R50] awk 求和
来源：http://mjk.guannengcc.top

awk '{s += $2} END {print s}' a.txt
来源：http://ued.shuidangran.top

[R51] 排序去重取前几
来源：http://cgr.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://kmx.sysykeji.top

[R52] 统计行数
来源：http://nup.xuetiantiany.cn

wc -l a.txt
来源：http://nyo.zycfv.cn

[R53] 查看文件头与实时尾
来源：http://wkp.316326.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kti.svipenyu.cn

[R54] 比较两个文件
来源：http://ewo.chenlongwang.top

diff a.txt b.txt
来源：http://hvq.jianghu66.top

[R55] 压缩与解压
来源：http://qod.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bzi.zhixingplan.top

[R56] 远程拷贝
来源：http://amz.chenjidiqi.icu

scp file user@host:/path/
来源：http://wph.wangdashe.top

[R57] 远程执行命令
来源：http://ctz.snrcjt.cn

ssh user@host 'uptime'
来源：http://lei.zhoulong.xyz

[R58] 下载文件
来源：http://jxw.hfpthk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nup.vehdjk.com

[R59] 发 POST JSON
来源：http://hoj.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fci.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://qkj.tanke756.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ksz.fehbvm.com

[R61] 磁盘占用
来源：http://mxs.smart0.xyz

df -h;  du -sh *
来源：http://yoa.uphjek.com

[R62] 找最占空间的文件
来源：http://bzt.yueranfly.top

du -ah . | sort -rh | head -10
来源：http://nia.iojbl.cn

[R63] 内存与进程
来源：http://fnr.quarkkingdee.top

free -h;  ps aux | grep nginx
来源：http://vkc.yanxiufei.cn

[R64] 结束进程
来源：http://esi.yonumen.top

kill -9 $(pgrep -f app.py)
来源：http://zxe.xuetiantiany.cn

[R65] 查看端口占用
来源：http://abu.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://igk.jinyuanbaomall.cn

[R66] 定时任务
来源：http://hei.fzhhl.top

crontab -e;  crontab -l
来源：http://uzl.fehbvm.com

[R67] 生成随机十六进制串
来源：http://zos.ydzc1.top

openssl rand -hex 16
来源：http://pak.chenlongwang.top

[R68] 计算文件校验值
来源：http://xab.wangdashe.top

sha256sum a.txt;  md5sum a.txt
来源：http://kzd.kuanghao11.cn

[R69] 生成随机密码
来源：http://gjs.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://omh.yanxiufei.cn

[R70] 时间戳与互转
来源：http://aih.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://afu.shangyingyoupin.top

[R71] 日期格式化
来源：http://fqb.hesvh.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lzu.jlsjyb.cn

[R72] 等待端口就绪
来源：http://tsy.ivvv.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kfo.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://ngf.gzhubu.top

split -l 1000 big.log part_
来源：http://sid.yvedp.cn

[R74] 批量重命名
来源：http://wnf.hongshengwenyu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ilw.feifeiyinyue.top

[R75] 导出环境变量
来源：http://rza.xziqi.cn

export PATH="$HOME/bin:$PATH"
来源：http://qqy.fehbvm.com

[R76] 使用临时文件
来源：http://xlk.cashguo.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nxo.zhaomingkeji.xyz

[R77] 读取用户输入
来源：http://omn.zhengqikj.top

read -rp "请输入: " ans
来源：http://epm.gotoacloud.top

[R78] 交互式菜单
来源：http://pcn.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gdv.jinyuanbaomall.cn

[R79] 解析命令行选项
来源：http://tgc.jianghu66.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oqt.yuxming.cn

[R80] 查看脚本执行耗时
来源：http://wup.9152youxi.cn

time ./run.sh
来源：http://kgf.xinyue.icu

================================================================================
来源：http://lwe.zhengqikj.top

S. C / C++ 专题
来源：http://gmb.shzxlz.cn

================================================================================
来源：http://eod.aibaodan.cn

[S01] C：Hello World
来源：http://csl.smart0.xyz

#include <stdio.h>
来源：http://tsd.xylfe.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wwl.birdmap.top

[S02] C：变量与格式化输出
来源：http://yoq.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://dbc.xziqi.cn

[S03] C：读入整数
来源：http://mfd.daxiang520.top

int x; scanf("%d", &x);
来源：http://eep.daxiang520.top

[S04] C：字符串复制
来源：http://guf.zhengqikj.top

char dst[32]; strcpy(dst, "hi");
来源：http://afd.vqdsnc.cn

[S05] C：字符串长度
来源：http://xwi.gzhubu.top

strlen(s)
来源：http://gtp.cqqwz.cn

[S06] C：字符串比较
来源：http://uph.yfazqb.com

strcmp(a, b) == 0
来源：http://lir.nanxinkj.top

[S07] C：数组遍历求和
来源：http://xpo.yfazqb.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://djv.ivvv.top

[S08] C：动态内存分配与释放
来源：http://nht.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gsw.nanxuanxn.top

[S09] C：结构体定义与初始化
来源：http://njb.mhx1999.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jwe.jiagoushi.top

[S10] C：指针与解引用
来源：http://xgr.hesvh.cn

int *p = &a;  *p = 5;
来源：http://kwc.tianlin.xyz

[S11] C：逐行读文件
来源：http://zmv.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://kxg.ybcxt.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wbd.dianchejie.cn

fclose(f);
来源：http://bby.yj20258.top

[S12] C：写文件
来源：http://bap.tarul.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iyn.sjlbkw.cn

[S13] C：宏定义
来源：http://qoc.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ppj.yonumen.top

[S14] C：枚举
来源：http://uax.zdbjq.cn

enum Color { RED, GREEN, BLUE };
来源：http://cht.52xcode.cn

[S15] C：类型转换
来源：http://qtn.jiagoushi.top

(double) a / b
来源：http://xph.epnwcf.com

[S16] C：位操作置位
来源：http://eca.sweek.top

x |= (1 << 3);
来源：http://xlo.zhixingplan.top

[S17] C：安全拼接字符串
来源：http://ftz.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lih.xziqi.cn

[S18] C：命令行参数
来源：http://awv.xziqi.cn

int main(int argc, char **argv)
来源：http://iia.quarkkingdee.top

[S19] C：快速排序
来源：http://ght.kuanghao11.cn

qsort(a, n, sizeof(int), cmp);
来源：http://plj.ctjpmb.com

[S20] C：二分查找
来源：http://hqj.nanxinkj.top


<!-- 参考信息 -->