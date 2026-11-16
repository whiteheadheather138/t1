代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mxq.dashuyun.cn

[Q52] 删除指定行
来源：http://cir.yanxiufei.cn

DELETE FROM users WHERE id = 10;
来源：http://xmh.ybcxt.top

[Q53] 按条件删除
来源：http://pib.snrcjt.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wsl.sxryk.cn

[Q54] 清空表
来源：http://via.shuidangran.top

TRUNCATE TABLE logs;
来源：http://amf.jiagoushi.top

[Q55] 排名（并列占位）
来源：http://shk.jinghuilouyu.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://cod.meibo888.top

[Q56] 密集排名（并列不占位）
来源：http://wgb.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hjv.ybcxt.top

[Q57] 行号
来源：http://yuq.hcnkem.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://owf.gzhubu.top

[Q58] 累计求和
来源：http://hqb.gotoacloud.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xqj.cashguo.top

[Q59] 分组内累计
来源：http://fpp.fzhhl.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://itz.birdmap.top

[Q60] 取上一行 / 下一行
来源：http://phv.shuidangran.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ymj.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dse.nanxuanxn.top

[Q61] 移动平均
来源：http://bbh.yj20258888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ggp.zhongyouzk.top

[Q62] 分组占比
来源：http://ugh.zhongyouzk.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://eyd.daria6918.cn

[Q63] 开启事务
来源：http://gcj.vehdjk.com

START TRANSACTION;                -- 或 BEGIN
来源：http://pcv.mhx1999.top

[Q64] 提交事务
来源：http://uzz.yfazqb.com

COMMIT;
来源：http://shv.xylfe.cn

[Q65] 回滚事务
来源：http://nlw.jinqigfzy.top

ROLLBACK;
来源：http://mcf.epnwcf.com

[Q66] 行锁查询
来源：http://oap.yangfankeji.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jwd.svipenyu.cn

[Q67] 设置隔离级别
来源：http://ppb.jinyuanbaomall.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vux.guowangkeji.top

[Q68] 保存点
来源：http://vij.316326.xyz

SAVEPOINT sp1;
来源：http://lmh.gotoacloud.top

ROLLBACK TO sp1;
来源：http://woa.wangdashe.top

[Q69] 查看执行计划
来源：http://yac.sjlbkw.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ipj.pycfn.com

[Q70] 更新统计信息
来源：http://bdj.tanke756.top

ANALYZE TABLE users;
来源：http://zwt.jqgfzy.top

[Q71] 查看建表语句
来源：http://bbp.sxryk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://twq.shzxlz.cn

[Q72] 查看索引
来源：http://lav.svipenyu.cn

SHOW INDEX FROM users;
来源：http://pvj.zdbjq.cn

[Q73] 查看表状态
来源：http://wsq.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://khn.daxiang520.top

[Q74] 强制使用索引
来源：http://kah.nanxinkj.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://lso.tarul.cn

[Q75] 日期格式化
来源：http://eax.sysykeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dwt.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hzd.bjfxy.top

[Q76] 按天统计
来源：http://udb.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lgx.yangfankeji.com

[Q77] 时间加减
来源：http://tef.jqgufenzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tyn.fengsongda.top

[Q78] 当前时间
来源：http://nhy.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jpz.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://nlm.xingfuxueyuan.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dul.hongshengwenyu.top

[Q80] 字符串截取
来源：http://yte.chenjidiqi.icu

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rom.zhiwuduotai.top

[Q81] 字符串替换
来源：http://bis.dashuyun.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ecz.hfpthk.cn

[Q82] 字符长度与字节长度
来源：http://dei.gaohongyu789.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jij.cucudq.cn

[Q83] 大小写转换
来源：http://bvy.52xcode.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kht.xinyue.icu

[Q84] 去除首尾空格
来源：http://gmn.jyoumei.cn

SELECT TRIM(name) FROM users;
来源：http://wwc.yj20258888.top

[Q85] 数值取整
来源：http://yyc.ehwqpu.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zbr.havefunace.top

[Q86] 读取 JSON 字段
来源：http://nvv.yj20258.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nao.nanxinkj.top

[Q87] JSON 字段做条件
来源：http://qar.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://opk.gogol.net.cn

[Q88] 行转列（条件聚合）
来源：http://olu.yvedp.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wsd.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://plu.ehwqpu.com

[Q89] 判断表是否存在
来源：http://sof.zhaomingkeji.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vxz.yfazqb.com

[Q90] 生成序号列
来源：http://aab.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tyr.9152youxi.cn

================================================================================
来源：http://den.xylfe.cn

R. Bash 专题
来源：http://odv.ywan-chungtsiang.top

================================================================================
来源：http://cwa.dashuyun.cn

[R01] shebang 与严格模式
来源：http://pwd.yj20258.top

#!/usr/bin/env bash
来源：http://bal.jinqigufen.top

set -euo pipefail
来源：http://rsd.hongshengwenyu.top

[R02] 变量赋值与使用
来源：http://axc.dashuyun.cn

name="Tom"; echo "$name"
来源：http://kzt.zhoulong.xyz

[R03] 只读变量
来源：http://ujj.jlsjyb.cn

readonly PI=3.14
来源：http://hoz.jinyuanbaomall.cn

[R04] 位置参数
来源：http://bsa.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tcm.tianlin.xyz

[R05] 参数默认值
来源：http://taa.zycfv.cn

name="${1:-default}"
来源：http://ulw.cdnleiting.top

[R06] 判断命令是否存在
来源：http://qeh.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://beg.jlsjyb.cn

[R07] if 判断文件
来源：http://twm.zdqjudy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://abn.shzxlz.cn

[R08] 数值比较
来源：http://eeu.hcnkem.com

if (( a > b )); then echo "a 更大"; fi
来源：http://fta.ywan-chungtsiang.top

[R09] 字符串比较
来源：http://ozd.hcnkem.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ddg.shanyushiyangtech.top

[R10] 正则匹配
来源：http://elj.chenzaomai.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://acp.ybcxt.top

[R11] case 多分支
来源：http://dtb.hnqzz.top

case "$1" in
来源：http://xhh.hcnkem.com

start) echo "启动" ;;
来源：http://srn.c1oappe.top

stop)  echo "停止" ;;
来源：http://jrj.gaohongyu789.top

*)     echo "未知命令" ;;
来源：http://vvt.tarul.cn

esac
来源：http://cha.wangshuangyany.cn

[R12] for 遍历文件
来源：http://bnu.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://vja.havefunace.top

[R13] for 计数循环
来源：http://asl.chenzaomai.com

for i in {1..10}; do echo "$i"; done
来源：http://kgl.chenjidiqi.icu

[R14] C 风格 for
来源：http://zvq.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cwo.havefunace.top

[R15] while 逐行读文件
来源：http://waf.guowangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xil.zycfv.cn

[R16] until 等待条件
来源：http://vqf.ydzc1.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://igv.shanyushiyangkeji.top

[R17] 数组定义与取值
来源：http://zxv.9152youxi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://dvv.hcnkem.com

[R18] 遍历数组
来源：http://vlb.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://idi.jqgufenzy.top

[R19] 数组长度
来源：http://nva.nwbrower.top

echo "${#arr[@]}"
来源：http://lvl.wangdashe.top

[R20] 关联数组（字典）
来源：http://wib.wangshuangyany.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mxs.cdnleiting.top

[R21] 字符串长度
来源：http://vpd.snrcjt.cn

echo "${#s}"
来源：http://bxb.tarul.cn

[R22] 截取子串
来源：http://siy.sjlbkw.cn

echo "${s:0:5}"
来源：http://hto.tian-w.cn

[R23] 字符串替换
来源：http://smw.dashuyun.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kpu.zhengqikj.top

[R24] 大小写转换
来源：http://jqw.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pqj.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://yub.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rox.zhijiandao.cn

[R26] 命令替换
来源：http://jru.jqgufenzy.top

now=$(date +%F); echo "$now"
来源：http://wmf.chenzaomai.com

[R27] 算术展开
来源：http://vss.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://yfo.52xcode.cn

[R28] 浮点运算
来源：http://nsy.yj20258.top

echo "scale=2; 10/3" | bc
来源：http://jvj.tianlin.xyz

[R29] 定义函数
来源：http://ziz.xylfe.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zop.dianchejie.cn

[R30] 函数返回状态码
来源：http://gbp.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://xny.ywan-chungtsiang.top

[R31] 局部变量
来源：http://ati.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://pbs.xylfe.cn

[R32] 参数个数校验
来源：http://bgr.pengpengdd.cyou

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ipo.jqgufenzy.top

[R33] 捕获错误并提示行号
来源：http://eze.epnwcf.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qep.zhoulong.xyz

[R34] 退出时清理
来源：http://nhh.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gmf.shuidangran.top

[R35] 后台执行并等待
来源：http://pmu.hnqzz.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rzz.gotoacloud.top

[R36] 并发执行多个任务
来源：http://kbl.52xcode.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vgt.hfpthk.cn

[R37] 把输出赋给变量
来源：http://oqz.chenlongwang.top

files=$(ls -1)
来源：http://upn.fktsv.cn

[R38] 管道串联
来源：http://xyk.bbcook.cn

cat a.txt | grep -i error | wc -l
来源：http://vyr.316326.xyz

[R39] 重定向标准输出与错误
来源：http://lnf.wangdashe.top

cmd > out.log 2>&1
来源：http://dsb.redwolf501.top

[R40] 追加写日志
来源：http://ley.fktsv.cn

echo "log" >> out.log
来源：http://zba.bjfxy.top

[R41] 丢弃输出
来源：http://qet.hcnkem.com

cmd >/dev/null 2>&1
来源：http://cbw.c1oappe.top

[R42] 输入重定向
来源：http://kjv.andypj.xyz

wc -l < a.txt
来源：http://dyo.guowangkeji.top

[R43] 按名字查找文件
来源：http://hyh.feifeiyinyue.top

find . -name "*.log" -type f
来源：http://rxl.cqqwz.cn

[R44] 按修改时间查找
来源：http://fal.zhixingplan.top

find . -mtime -7 -type f
来源：http://flz.bjfxy.top

[R45] 批量删除
来源：http://rzu.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://yrb.yangfankeji.com

[R46] 递归替换文件内容
来源：http://xle.hcnkem.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vfg.yfazqb.com

[R47] sed 单行替换
来源：http://ndp.xuanzx.com

sed -i 's/foo/bar/g' a.txt
来源：http://fzt.cheryme.top

[R48] awk 取指定列
来源：http://lhg.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://uol.jqgufenzy.top

[R49] awk 带条件
来源：http://bhj.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xuo.hcnkem.com

[R50] awk 求和
来源：http://vhg.zhixingplan.top

awk '{s += $2} END {print s}' a.txt
来源：http://mqg.zdqjudy.top

[R51] 排序去重取前几
来源：http://qhz.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://htl.jqgfzy.top

[R52] 统计行数
来源：http://jfu.hongshengwenyu.top

wc -l a.txt
来源：http://ssl.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://rzr.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dwk.haohaochexian.top

[R54] 比较两个文件
来源：http://qne.yuanzhike.top

diff a.txt b.txt
来源：http://uqi.zdqjudy.top

[R55] 压缩与解压
来源：http://atn.zhiwuduotai.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ltv.52xcode.cn

[R56] 远程拷贝
来源：http://qzq.aizwys.cn

scp file user@host:/path/
来源：http://cur.zhoulong.xyz

[R57] 远程执行命令
来源：http://kqs.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://ymj.epnwcf.com

[R58] 下载文件
来源：http://pxd.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rek.snrcjt.cn

[R59] 发 POST JSON
来源：http://eot.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pdw.52xcode.cn

[R60] 只看 HTTP 状态码
来源：http://pwh.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hjg.hongshengwenyu.top

[R61] 磁盘占用
来源：http://ert.yfazqb.com

df -h;  du -sh *
来源：http://xnr.dashuyun.cn

[R62] 找最占空间的文件
来源：http://wsk.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://xgg.dianchejie.cn

[R63] 内存与进程
来源：http://bcv.c1oappe.top

free -h;  ps aux | grep nginx
来源：http://tlb.jianghu66.top

[R64] 结束进程
来源：http://oed.yuxming.cn

kill -9 $(pgrep -f app.py)
来源：http://krq.jyoumei.cn

[R65] 查看端口占用
来源：http://epu.c1oappe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://lij.sjlbkw.cn

[R66] 定时任务
来源：http://djz.jyoumei.cn

crontab -e;  crontab -l
来源：http://eif.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://nrx.hcnkem.com

openssl rand -hex 16
来源：http://vpp.hnqzz.top

[R68] 计算文件校验值
来源：http://rqk.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://ite.nanxuanxn.top

[R69] 生成随机密码
来源：http://ttp.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://wdi.yj20258888.top

[R70] 时间戳与互转
来源：http://zwy.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://mwz.hcnkem.com

[R71] 日期格式化
来源：http://vjj.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://iez.gzhubu.top

[R72] 等待端口就绪
来源：http://kkm.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://pfb.xinyue.icu

[R73] 分割大日志
来源：http://bgx.pengpengdd.cyou

split -l 1000 big.log part_
来源：http://rxm.52xcode.cn

[R74] 批量重命名
来源：http://btk.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wac.ywan-chungtsiang.top

[R75] 导出环境变量
来源：http://lis.yanxiufei.cn

export PATH="$HOME/bin:$PATH"
来源：http://ofn.zycfv.cn

[R76] 使用临时文件
来源：http://aum.ppjwa.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qop.ybcxt.top

[R77] 读取用户输入
来源：http://bel.jqgufenzy.top

read -rp "请输入: " ans
来源：http://vjy.shangyingyoupin.top

[R78] 交互式菜单
来源：http://fmb.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tey.chenzaomai.com

[R79] 解析命令行选项
来源：http://edn.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kwa.zhiwuduotai.top

[R80] 查看脚本执行耗时
来源：http://tvi.hywenlv.cn

time ./run.sh
来源：http://gcu.xylfe.cn

================================================================================
来源：http://jwl.yj20258.top

S. C / C++ 专题
来源：http://oou.zycfv.cn

================================================================================
来源：http://xxx.dashuyun.cn

[S01] C：Hello World
来源：http://kny.zhoulong.xyz

#include <stdio.h>
来源：http://pdc.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://tej.zdbjq.cn

[S02] C：变量与格式化输出
来源：http://esq.sysykeji.top

int a = 10; printf("%d\n", a);
来源：http://uve.zhijiandao.cn

[S03] C：读入整数
来源：http://xsz.smart0.xyz

int x; scanf("%d", &x);
来源：http://yix.shzxlz.cn

[S04] C：字符串复制
来源：http://clg.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://ozr.gogol.net.cn

[S05] C：字符串长度
来源：http://mhx.hfpthk.cn

strlen(s)
来源：http://acq.quarkkingdee.top

[S06] C：字符串比较
来源：http://ynn.hfpthk.cn

strcmp(a, b) == 0
来源：http://ymr.ivvv.top

[S07] C：数组遍历求和
来源：http://ogd.kuanghao11.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yae.yonumen.top

[S08] C：动态内存分配与释放
来源：http://zvv.zdqjudy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yac.hysaishi.cn

[S09] C：结构体定义与初始化
来源：http://unz.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://utl.9152youxi.cn

[S10] C：指针与解引用
来源：http://wxa.cdnleiting.top

int *p = &a;  *p = 5;
来源：http://jqb.chenlongwang.top

[S11] C：逐行读文件
来源：http://orq.hammf.cn

FILE *f = fopen("a.txt", "r");
来源：http://egd.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jht.zhengqikj.top

fclose(f);
来源：http://wwa.316326.xyz

[S12] C：写文件
来源：http://mfi.hysaishi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zkf.smart0.xyz

[S13] C：宏定义
来源：http://xjc.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wnl.vqdsnc.cn

[S14] C：枚举
来源：http://szb.ydjk.org.cn

enum Color { RED, GREEN, BLUE };
来源：http://sxv.pengpengdd.cyou

[S15] C：类型转换
来源：http://uul.iojbl.cn

(double) a / b
来源：http://ebn.zdqjudy.top

[S16] C：位操作置位
来源：http://evs.guannengcc.top

x |= (1 << 3);
来源：http://zcj.zdqjudy.top

[S17] C：安全拼接字符串
来源：http://elz.tianlin.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bcm.316326.xyz

[S18] C：命令行参数
来源：http://tqh.jiagoushi.top

int main(int argc, char **argv)
来源：http://jbc.quarkkingdee.top

[S19] C：快速排序
来源：http://fvv.fzhhl.top

qsort(a, n, sizeof(int), cmp);
来源：http://ahr.quarkkingdee.top

[S20] C：二分查找
来源：http://cms.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jvc.bbcook.cn

[S21] C：字符类别判断
来源：http://rzh.yangfankeji.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cbk.xziqi.cn

[S22] C：字符串转数字
来源：http://kvv.pengpengdd.cyou


<!-- 参考信息 -->