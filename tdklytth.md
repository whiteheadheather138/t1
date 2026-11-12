代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ser.wangdashe.top

[Q50] 批量更新
来源：http://igb.zhijiandao.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://adi.bbcook.cn

[Q51] 用子查询更新
来源：http://zyf.jqgufenzy.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lgf.sysykeji.top

[Q52] 删除指定行
来源：http://wqq.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://mbd.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://fai.yfazqb.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ddc.ehwqpu.com

[Q54] 清空表
来源：http://fvf.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://byt.tianlin.xyz

[Q55] 排名（并列占位）
来源：http://amt.cucudq.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cay.jyoumei.cn

[Q56] 密集排名（并列不占位）
来源：http://ijb.svipenyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hdv.hcnkem.com

[Q57] 行号
来源：http://kfz.shuidangran.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hks.bbcook.cn

[Q58] 累计求和
来源：http://lex.zhijiandao.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://udh.cheryme.top

[Q59] 分组内累计
来源：http://evz.tarul.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ykc.shangyingyoupin.top

[Q60] 取上一行 / 下一行
来源：http://bsr.nwbrower.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qei.c1oappe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cyg.xziqi.cn

[Q61] 移动平均
来源：http://wxo.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pwf.fanxiaobao.xyz

[Q62] 分组占比
来源：http://ckb.gaohongyu789.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://giq.ppjwa.cn

[Q63] 开启事务
来源：http://vwm.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://cff.sxryk.cn

[Q64] 提交事务
来源：http://tde.ppjwa.cn

COMMIT;
来源：http://nyg.cdnleiting.top

[Q65] 回滚事务
来源：http://pqu.meibo888.top

ROLLBACK;
来源：http://yea.chenzaomai.com

[Q66] 行锁查询
来源：http://kaf.sufxvd.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zwn.pycfn.com

[Q67] 设置隔离级别
来源：http://uiy.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://qut.snrcjt.cn

[Q68] 保存点
来源：http://mdh.hywenlv.cn

SAVEPOINT sp1;
来源：http://hxm.yj20258888.top

ROLLBACK TO sp1;
来源：http://jyq.yueranfly.top

[Q69] 查看执行计划
来源：http://kyf.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://crx.hesvh.cn

[Q70] 更新统计信息
来源：http://ktu.shzxlz.cn

ANALYZE TABLE users;
来源：http://kol.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://sog.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://car.52xcode.cn

[Q72] 查看索引
来源：http://dko.yj20258888.top

SHOW INDEX FROM users;
来源：http://ure.cashguo.top

[Q73] 查看表状态
来源：http://rrc.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://bnc.yvedp.cn

[Q74] 强制使用索引
来源：http://wum.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://erf.wangshuangyany.cn

[Q75] 日期格式化
来源：http://zth.zhengqikj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://avt.jianghu66.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cyf.dianchejie.cn

[Q76] 按天统计
来源：http://pai.fehbvm.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://izb.fzhhl.top

[Q77] 时间加减
来源：http://bwc.ydjk.org.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jxq.hfpthk.cn

[Q78] 当前时间
来源：http://fuu.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kde.yueranfly.top

[Q79] 字符串拼接
来源：http://ioy.zhixingplan.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eca.zhiwuduotai.top

[Q80] 字符串截取
来源：http://rkc.shuidangran.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wic.ivvv.top

[Q81] 字符串替换
来源：http://swu.yfazqb.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dbv.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://jcr.hfpthk.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eij.daxiang520.top

[Q83] 大小写转换
来源：http://rtf.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jin.nanxinkj.top

[Q84] 去除首尾空格
来源：http://max.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://lfr.vehdjk.com

[Q85] 数值取整
来源：http://mkp.yuxming.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jid.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://act.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oqq.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://wbk.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vlv.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://jmg.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dtl.gaohongyu789.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wlr.tarul.cn

[Q89] 判断表是否存在
来源：http://kkr.yangfankeji.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ftu.aibaodan.cn

[Q90] 生成序号列
来源：http://ofo.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pja.ydzc1.top

================================================================================
来源：http://bxk.cashguo.top

R. Bash 专题
来源：http://nll.smart0.xyz

================================================================================
来源：http://hqp.svipenyu.cn

[R01] shebang 与严格模式
来源：http://koy.jlsjyb.cn

#!/usr/bin/env bash
来源：http://tcg.yj202588.top

set -euo pipefail
来源：http://qgp.yonumen.top

[R02] 变量赋值与使用
来源：http://ait.ctjpmb.com

name="Tom"; echo "$name"
来源：http://kdb.shanyushiyangtech.top

[R03] 只读变量
来源：http://whp.ywan-chungtsiang.top

readonly PI=3.14
来源：http://kqn.zycfv.cn

[R04] 位置参数
来源：http://lek.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://upx.zdqjudy.top

[R05] 参数默认值
来源：http://xhq.52xcode.cn

name="${1:-default}"
来源：http://phm.xingfuxueyuan.xyz

[R06] 判断命令是否存在
来源：http://xjd.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://azx.fengsongda.top

[R07] if 判断文件
来源：http://mqg.birdmap.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ipt.jqgufenzy.top

[R08] 数值比较
来源：http://bya.daxiang520.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rtd.nanxinkj.top

[R09] 字符串比较
来源：http://rsj.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pgj.vehdjk.com

[R10] 正则匹配
来源：http://kaz.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lef.9152youxi.cn

[R11] case 多分支
来源：http://arj.gogol.net.cn

case "$1" in
来源：http://uaw.havefunace.top

start) echo "启动" ;;
来源：http://ygx.zdqjudy.top

stop)  echo "停止" ;;
来源：http://mvf.yuanzhike.top

*)     echo "未知命令" ;;
来源：http://czl.birdmap.top

esac
来源：http://lmc.cucudq.cn

[R12] for 遍历文件
来源：http://dyu.cqqwz.cn

for f in *.txt; do echo "$f"; done
来源：http://mut.sxryk.cn

[R13] for 计数循环
来源：http://zby.uphjek.com

for i in {1..10}; do echo "$i"; done
来源：http://jhl.yj202588.top

[R14] C 风格 for
来源：http://gtv.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xue.shanyushiyangkeji.top

[R15] while 逐行读文件
来源：http://vhd.yj202588.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://yzg.haohaochexian.top

[R16] until 等待条件
来源：http://feg.ehwqpu.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pgq.xinyue.icu

[R17] 数组定义与取值
来源：http://gzw.daria6918.cn

arr=(a b c); echo "${arr[0]}"
来源：http://hhw.zhengqikj.top

[R18] 遍历数组
来源：http://vuf.ppjwa.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bpv.feifeiyinyue.top

[R19] 数组长度
来源：http://rua.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://lyf.andypj.xyz

[R20] 关联数组（字典）
来源：http://kwu.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qet.aizwys.cn

[R21] 字符串长度
来源：http://res.xuetiantiany.cn

echo "${#s}"
来源：http://swn.jianghu66.top

[R22] 截取子串
来源：http://kfy.vehdjk.com

echo "${s:0:5}"
来源：http://tyw.vehdjk.com

[R23] 字符串替换
来源：http://gvn.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://xeq.yonumen.top

[R24] 大小写转换
来源：http://zyu.xziqi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bgb.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://ptm.zhoulong.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://uvw.fzhhl.top

[R26] 命令替换
来源：http://egi.jlsjyb.cn

now=$(date +%F); echo "$now"
来源：http://aav.ctjpmb.com

[R27] 算术展开
来源：http://ygu.zycfv.cn

echo $((1 + 2 * 3))
来源：http://rig.wangdashe.top

[R28] 浮点运算
来源：http://wid.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://tku.yj202588.top

[R29] 定义函数
来源：http://upc.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://scp.shanyushiyangkeji.top

[R30] 函数返回状态码
来源：http://nnf.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://vdl.pycfn.com

[R31] 局部变量
来源：http://yfe.nanxinkj.top

f() { local x=1; echo "$x"; }
来源：http://mth.pengpengdd.cyou

[R32] 参数个数校验
来源：http://rwl.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rij.fehbvm.com

[R33] 捕获错误并提示行号
来源：http://lvf.sxryk.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://atm.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://zsw.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://zci.sweek.top

[R35] 后台执行并等待
来源：http://mup.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://svg.sweek.top

[R36] 并发执行多个任务
来源：http://lgk.jqgfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkx.zhixingplan.top

[R37] 把输出赋给变量
来源：http://rft.vqdsnc.cn

files=$(ls -1)
来源：http://wyr.dashuyun.cn

[R38] 管道串联
来源：http://cuh.birdmap.top

cat a.txt | grep -i error | wc -l
来源：http://ljg.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://wnp.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://ybo.haohaochexian.top

[R40] 追加写日志
来源：http://tbf.kuanghao11.cn

echo "log" >> out.log
来源：http://lad.yfazqb.com

[R41] 丢弃输出
来源：http://lgr.316326.xyz

cmd >/dev/null 2>&1
来源：http://faj.jianghu66.top

[R42] 输入重定向
来源：http://zcr.ydzc1.top

wc -l < a.txt
来源：http://pst.gzhubu.top

[R43] 按名字查找文件
来源：http://ose.hcnkem.com

find . -name "*.log" -type f
来源：http://zry.nanxinkj.top

[R44] 按修改时间查找
来源：http://uce.cdnleiting.top

find . -mtime -7 -type f
来源：http://nwk.chenlongwang.top

[R45] 批量删除
来源：http://gnv.xuanzx.com

find . -name "*.tmp" -delete
来源：http://mld.andypj.xyz

[R46] 递归替换文件内容
来源：http://wzs.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qln.uphjek.com

[R47] sed 单行替换
来源：http://xep.tian-w.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uvu.zhengqikj.top

[R48] awk 取指定列
来源：http://pso.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://gaq.yangfankeji.com

[R49] awk 带条件
来源：http://pxr.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://boh.yj20258.top

[R50] awk 求和
来源：http://wku.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://qya.aizwys.cn

[R51] 排序去重取前几
来源：http://vum.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zoy.aibaodan.cn

[R52] 统计行数
来源：http://yvl.yj20258888.top

wc -l a.txt
来源：http://adv.zdqjudy.top

[R53] 查看文件头与实时尾
来源：http://ilf.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sek.guowangkeji.top

[R54] 比较两个文件
来源：http://nhc.yuanzhike.top

diff a.txt b.txt
来源：http://wcu.0kj1m.cn

[R55] 压缩与解压
来源：http://okc.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oax.316326.xyz

[R56] 远程拷贝
来源：http://xtr.jqgfzy.top

scp file user@host:/path/
来源：http://aht.gogol.net.cn

[R57] 远程执行命令
来源：http://ilu.iojbl.cn

ssh user@host 'uptime'
来源：http://nzo.shanyushiyangtech.top

[R58] 下载文件
来源：http://wfz.zhaomingkeji.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xjl.chenlongwang.top

[R59] 发 POST JSON
来源：http://hxo.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ibg.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://dvy.pycfn.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hsz.vehdjk.com

[R61] 磁盘占用
来源：http://nii.zycfv.cn

df -h;  du -sh *
来源：http://lep.ivvv.top

[R62] 找最占空间的文件
来源：http://bnq.hesvh.cn

du -ah . | sort -rh | head -10
来源：http://qzl.daria6918.cn

[R63] 内存与进程
来源：http://giq.zhongyouzk.top

free -h;  ps aux | grep nginx
来源：http://wql.hcnkem.com

[R64] 结束进程
来源：http://uyv.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://eas.sysykeji.top

[R65] 查看端口占用
来源：http://xtt.jinqigufen.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sjf.haohaochexian.top

[R66] 定时任务
来源：http://dge.yongpay.top

crontab -e;  crontab -l
来源：http://qtt.yonumen.top

[R67] 生成随机十六进制串
来源：http://hri.hammf.cn

openssl rand -hex 16
来源：http://upy.haohaochexian.top

[R68] 计算文件校验值
来源：http://qht.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://zsa.iojbl.cn

[R69] 生成随机密码
来源：http://kfz.fzhhl.top

head -c 16 /dev/urandom | base64
来源：http://qdl.daxiang520.top

[R70] 时间戳与互转
来源：http://hbt.kuanghao11.cn

date +%s;  date -d @1700000000
来源：http://rhk.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://hvz.wangdashe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mjl.kuanghao11.cn

[R72] 等待端口就绪
来源：http://rzr.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nar.yj202588.top

[R73] 分割大日志
来源：http://yua.sjlbkw.cn

split -l 1000 big.log part_
来源：http://pdh.fehbvm.com

[R74] 批量重命名
来源：http://ttn.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ppx.fengsongda.top

[R75] 导出环境变量
来源：http://fjt.nanxuanxn.top

export PATH="$HOME/bin:$PATH"
来源：http://uae.hcnkem.com

[R76] 使用临时文件
来源：http://mnl.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://imk.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://ffa.andypj.xyz

read -rp "请输入: " ans
来源：http://jts.dianchejie.cn

[R78] 交互式菜单
来源：http://eil.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ooj.yanxiufei.cn

[R79] 解析命令行选项
来源：http://qpd.ehwqpu.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rxx.xziqi.cn

[R80] 查看脚本执行耗时
来源：http://fhk.sweek.top

time ./run.sh
来源：http://qmy.nanxuanxn.top

================================================================================
来源：http://kcq.ctjpmb.com

S. C / C++ 专题
来源：http://ckl.daria6918.cn

================================================================================
来源：http://jbd.hywenlv.cn

[S01] C：Hello World
来源：http://rnb.hammf.cn

#include <stdio.h>
来源：http://iwn.hysaishi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://obh.xuanzx.com

[S02] C：变量与格式化输出
来源：http://gwh.chenlongwang.top

int a = 10; printf("%d\n", a);
来源：http://mwi.xingfuxueyuan.xyz

[S03] C：读入整数
来源：http://dmk.yangfankeji.com

int x; scanf("%d", &x);
来源：http://xyo.shangyingyoupin.top

[S04] C：字符串复制
来源：http://cmf.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://tsc.sysykeji.top

[S05] C：字符串长度
来源：http://nqs.sweek.top

strlen(s)
来源：http://gir.zhijiandao.cn

[S06] C：字符串比较
来源：http://ayo.jinqigfzy.top

strcmp(a, b) == 0
来源：http://kmo.c1oappe.top

[S07] C：数组遍历求和
来源：http://jxh.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://isj.redwolf501.top

[S08] C：动态内存分配与释放
来源：http://fsy.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vkp.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://xev.dianchejie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kji.ybcxt.top

[S10] C：指针与解引用
来源：http://mcf.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://svr.yj202588.top

[S11] C：逐行读文件
来源：http://csu.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ybb.ywan-chungtsiang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://igd.hywenlv.cn

fclose(f);
来源：http://zvh.fanxiaobao.xyz

[S12] C：写文件
来源：http://eqm.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nsm.jinqigufen.top

[S13] C：宏定义
来源：http://gil.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dro.fehbvm.com

[S14] C：枚举
来源：http://icc.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://qdw.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://hus.zhiwuduotai.top

(double) a / b
来源：http://cqj.yj20258.top

[S16] C：位操作置位
来源：http://dls.hongshengwenyu.top

x |= (1 << 3);
来源：http://ydi.yuanzhike.top

[S17] C：安全拼接字符串
来源：http://fpw.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://imb.sjlbkw.cn

[S18] C：命令行参数
来源：http://lge.jlsjyb.cn

int main(int argc, char **argv)
来源：http://chj.feifeiyinyue.top

[S19] C：快速排序
来源：http://tvc.vqdsnc.cn

qsort(a, n, sizeof(int), cmp);
来源：http://slo.wangdashe.top

[S20] C：二分查找
来源：http://ooc.gzhubu.top


<!-- 参考信息 -->