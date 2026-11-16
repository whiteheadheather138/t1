代发 wailian999

[Q63] 开启事务
来源：http://tjj.ivvv.top

START TRANSACTION;                -- 或 BEGIN
来源：http://nqw.zhaomingkeji.xyz

[Q64] 提交事务
来源：http://nzv.quarkkingdee.top

COMMIT;
来源：http://xzf.fehbvm.com

[Q65] 回滚事务
来源：http://gex.zhiwuduotai.top

ROLLBACK;
来源：http://zvf.gaohongyu789.top

[Q66] 行锁查询
来源：http://otu.ctjpmb.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gbm.wangdashe.top

[Q67] 设置隔离级别
来源：http://ofy.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://cds.jianghu66.top

[Q68] 保存点
来源：http://gze.zhengqikj.top

SAVEPOINT sp1;
来源：http://ban.yuxming.cn

ROLLBACK TO sp1;
来源：http://cxl.sufxvd.cn

[Q69] 查看执行计划
来源：http://upi.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tws.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://amr.yonumen.top

ANALYZE TABLE users;
来源：http://efg.zhixingplan.top

[Q71] 查看建表语句
来源：http://yyb.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qdu.yueranfly.top

[Q72] 查看索引
来源：http://kqi.yj20258.top

SHOW INDEX FROM users;
来源：http://irr.c1oappe.top

[Q73] 查看表状态
来源：http://hyd.jinqigfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://fss.zhixingplan.top

[Q74] 强制使用索引
来源：http://bbe.iojbl.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://amz.haohaochexian.top

[Q75] 日期格式化
来源：http://gct.tanke756.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sek.jinghuilouyu.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://etc.zhixingplan.top

[Q76] 按天统计
来源：http://cad.cdnleiting.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zrm.chenjidiqi.icu

[Q77] 时间加减
来源：http://uhl.yueranfly.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://bxi.feifeiyinyue.top

[Q78] 当前时间
来源：http://vyj.tanke756.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hvn.jianghu66.top

[Q79] 字符串拼接
来源：http://oln.zhiwuduotai.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://kwt.uphjek.com

[Q80] 字符串截取
来源：http://fgq.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xxj.yj202588.top

[Q81] 字符串替换
来源：http://vak.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rpn.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://okm.jqgfzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bcc.ppjwa.cn

[Q83] 大小写转换
来源：http://lnl.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uxh.svipenyu.cn

[Q84] 去除首尾空格
来源：http://xou.epnwcf.com

SELECT TRIM(name) FROM users;
来源：http://jei.hnxiangtu.top

[Q85] 数值取整
来源：http://fru.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ugd.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://ozq.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zgy.dashuyun.cn

[Q87] JSON 字段做条件
来源：http://fvm.ehwqpu.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ntn.shuidangran.top

[Q88] 行转列（条件聚合）
来源：http://evz.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wic.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fda.hcnkem.com

[Q89] 判断表是否存在
来源：http://gat.uphjek.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ulx.jqgufenzy.top

[Q90] 生成序号列
来源：http://ncx.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ntg.wangshuangyany.cn

================================================================================
来源：http://azh.zhijiandao.cn

R. Bash 专题
来源：http://fpo.ywan-chungtsiang.top

================================================================================
来源：http://cqc.ydzc1.top

[R01] shebang 与严格模式
来源：http://sxy.nwbrower.top

#!/usr/bin/env bash
来源：http://kqr.guowangkeji.top

set -euo pipefail
来源：http://ygv.aizwys.cn

[R02] 变量赋值与使用
来源：http://otq.jinghuilouyu.cn

name="Tom"; echo "$name"
来源：http://isy.jqgufenzy.top

[R03] 只读变量
来源：http://uiu.0kj1m.cn

readonly PI=3.14
来源：http://awu.sjlbkw.cn

[R04] 位置参数
来源：http://pzt.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dhi.hywenlv.cn

[R05] 参数默认值
来源：http://mew.jiagoushi.top

name="${1:-default}"
来源：http://zij.sweek.top

[R06] 判断命令是否存在
来源：http://ggp.nanxinkj.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://bej.meibo888.top

[R07] if 判断文件
来源：http://loy.aizwys.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://thx.svipenyu.cn

[R08] 数值比较
来源：http://jqf.yueranfly.top

if (( a > b )); then echo "a 更大"; fi
来源：http://fxw.316326.xyz

[R09] 字符串比较
来源：http://yua.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qhl.yueranfly.top

[R10] 正则匹配
来源：http://snu.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jqg.hammf.cn

[R11] case 多分支
来源：http://aba.pengpengdd.cyou

case "$1" in
来源：http://eed.52xcode.cn

start) echo "启动" ;;
来源：http://zhp.ehwqpu.com

stop)  echo "停止" ;;
来源：http://cyy.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://krh.0kj1m.cn

esac
来源：http://snm.shangyingyoupin.top

[R12] for 遍历文件
来源：http://ywd.daria6918.cn

for f in *.txt; do echo "$f"; done
来源：http://pwa.andypj.xyz

[R13] for 计数循环
来源：http://rqh.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://cyd.daxiang520.top

[R14] C 风格 for
来源：http://mvu.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pkh.xinyue.icu

[R15] while 逐行读文件
来源：http://guz.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fyr.gaohongyu789.top

[R16] until 等待条件
来源：http://zgz.mhx1999.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cuu.jinqigufen.top

[R17] 数组定义与取值
来源：http://bvx.hywenlv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sgw.chenjidiqi.icu

[R18] 遍历数组
来源：http://bux.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dot.chenzaomai.com

[R19] 数组长度
来源：http://xbv.cheryme.top

echo "${#arr[@]}"
来源：http://pkr.nwbrower.top

[R20] 关联数组（字典）
来源：http://gvf.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rgd.ivvv.top

[R21] 字符串长度
来源：http://nzz.haohaochexian.top

echo "${#s}"
来源：http://vvg.hywenlv.cn

[R22] 截取子串
来源：http://xqg.nwbrower.top

echo "${s:0:5}"
来源：http://gjy.hnqzz.top

[R23] 字符串替换
来源：http://lyx.gogol.net.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dck.zycfv.cn

[R24] 大小写转换
来源：http://wtr.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://ouh.feifeiyinyue.top

[R25] 去后缀 / 去前缀
来源：http://odv.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ibo.hongshengwenyu.top

[R26] 命令替换
来源：http://wpp.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://anb.chenzaomai.com

[R27] 算术展开
来源：http://qcm.hywenlv.cn

echo $((1 + 2 * 3))
来源：http://rqk.zdqjudy.top

[R28] 浮点运算
来源：http://uzy.guannengcc.top

echo "scale=2; 10/3" | bc
来源：http://orm.tanke756.top

[R29] 定义函数
来源：http://tmh.yj20258.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://luh.ywan-chungtsiang.top

[R30] 函数返回状态码
来源：http://chf.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://xvh.kuanghao11.cn

[R31] 局部变量
来源：http://shy.chenzaomai.com

f() { local x=1; echo "$x"; }
来源：http://dqj.nanxuanxn.top

[R32] 参数个数校验
来源：http://uaq.xuanzx.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kjf.havefunace.top

[R33] 捕获错误并提示行号
来源：http://dva.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qog.cdnleiting.top

[R34] 退出时清理
来源：http://cnn.ydjk.org.cn

trap 'rm -f "$tmp"' EXIT
来源：http://zrf.yj202588.top

[R35] 后台执行并等待
来源：http://bdz.xingfuxueyuan.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://xaa.sweek.top

[R36] 并发执行多个任务
来源：http://una.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cgd.nwbrower.top

[R37] 把输出赋给变量
来源：http://vsx.cheryme.top

files=$(ls -1)
来源：http://isv.svipenyu.cn

[R38] 管道串联
来源：http://esw.jinghuilouyu.cn

cat a.txt | grep -i error | wc -l
来源：http://iyu.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://bve.haohaochexian.top

cmd > out.log 2>&1
来源：http://cpu.jinqigufen.top

[R40] 追加写日志
来源：http://yxw.yuanzhike.top

echo "log" >> out.log
来源：http://lej.yanxiufei.cn

[R41] 丢弃输出
来源：http://fad.fktsv.cn

cmd >/dev/null 2>&1
来源：http://oab.hfpthk.cn

[R42] 输入重定向
来源：http://kct.zdbjq.cn

wc -l < a.txt
来源：http://geu.pengpengdd.cyou

[R43] 按名字查找文件
来源：http://qew.nanxuanxn.top

find . -name "*.log" -type f
来源：http://dml.sysykeji.top

[R44] 按修改时间查找
来源：http://ofc.52xcode.cn

find . -mtime -7 -type f
来源：http://kop.svipenyu.cn

[R45] 批量删除
来源：http://uwj.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://fdr.9152youxi.cn

[R46] 递归替换文件内容
来源：http://lac.xinyue.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wth.xziqi.cn

[R47] sed 单行替换
来源：http://vgn.jiagoushi.top

sed -i 's/foo/bar/g' a.txt
来源：http://fvw.havefunace.top

[R48] awk 取指定列
来源：http://vbh.shzxlz.cn

awk '{print $1, $3}' a.txt
来源：http://tjw.vqdsnc.cn

[R49] awk 带条件
来源：http://lfy.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mmt.bbcook.cn

[R50] awk 求和
来源：http://mcs.nanxinkj.top

awk '{s += $2} END {print s}' a.txt
来源：http://xrr.zhoulong.xyz

[R51] 排序去重取前几
来源：http://lfg.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://daf.fehbvm.com

[R52] 统计行数
来源：http://zua.jqgufenzy.top

wc -l a.txt
来源：http://ein.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://uqt.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jdi.zhiwuduotai.top

[R54] 比较两个文件
来源：http://jfg.sjlbkw.cn

diff a.txt b.txt
来源：http://zmr.hysaishi.cn

[R55] 压缩与解压
来源：http://ugu.chenjidiqi.icu

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fko.shuidangran.top

[R56] 远程拷贝
来源：http://cld.zhijiandao.cn

scp file user@host:/path/
来源：http://bfb.shzxlz.cn

[R57] 远程执行命令
来源：http://wvb.sysykeji.top

ssh user@host 'uptime'
来源：http://hgl.tarul.cn

[R58] 下载文件
来源：http://sno.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bet.ehwqpu.com

[R59] 发 POST JSON
来源：http://yov.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uwa.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://tvl.cucudq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hgy.meibo888.top

[R61] 磁盘占用
来源：http://bus.zhijiandao.cn

df -h;  du -sh *
来源：http://ijr.c1oappe.top

[R62] 找最占空间的文件
来源：http://cxr.epnwcf.com

du -ah . | sort -rh | head -10
来源：http://pwz.kuanghao11.cn

[R63] 内存与进程
来源：http://ule.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://cyf.zdbjq.cn

[R64] 结束进程
来源：http://yvi.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://ymm.cdnleiting.top

[R65] 查看端口占用
来源：http://jot.tianlin.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rqz.zdbjq.cn

[R66] 定时任务
来源：http://ysw.9152youxi.cn

crontab -e;  crontab -l
来源：http://jem.bbcook.cn

[R67] 生成随机十六进制串
来源：http://fro.shangyingyoupin.top

openssl rand -hex 16
来源：http://ynq.cdnleiting.top

[R68] 计算文件校验值
来源：http://fbp.hcnkem.com

sha256sum a.txt;  md5sum a.txt
来源：http://umt.zycfv.cn

[R69] 生成随机密码
来源：http://zsi.dianchejie.cn

head -c 16 /dev/urandom | base64
来源：http://uum.birdmap.top

[R70] 时间戳与互转
来源：http://fll.bjfxy.top

date +%s;  date -d @1700000000
来源：http://qxf.pycfn.com

[R71] 日期格式化
来源：http://yak.daria6918.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yjv.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://ujb.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rcl.xingfuxueyuan.xyz

[R73] 分割大日志
来源：http://nva.ybcxt.top

split -l 1000 big.log part_
来源：http://yur.pycfn.com

[R74] 批量重命名
来源：http://vug.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zdl.ivvv.top

[R75] 导出环境变量
来源：http://miu.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://cdj.jqgfzy.top

[R76] 使用临时文件
来源：http://hua.nanxinkj.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ebd.zhengqikj.top

[R77] 读取用户输入
来源：http://xzo.wangdashe.top

read -rp "请输入: " ans
来源：http://jba.fktsv.cn

[R78] 交互式菜单
来源：http://igx.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ebw.fzhhl.top

[R79] 解析命令行选项
来源：http://txp.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zkh.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://lcy.hnqzz.top

time ./run.sh
来源：http://ahk.yongpay.top

================================================================================
来源：http://ekg.yuanzhike.top

S. C / C++ 专题
来源：http://srm.nanxuanxn.top

================================================================================
来源：http://ogm.uphjek.com

[S01] C：Hello World
来源：http://ytp.xuanzx.com

#include <stdio.h>
来源：http://ppq.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hcq.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://mff.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://lzn.hammf.cn

[S03] C：读入整数
来源：http://xyo.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://wxg.hcnkem.com

[S04] C：字符串复制
来源：http://pap.bbcook.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zbv.svipenyu.cn

[S05] C：字符串长度
来源：http://qwx.52xcode.cn

strlen(s)
来源：http://nml.jqgufenzy.top

[S06] C：字符串比较
来源：http://nix.zycfv.cn

strcmp(a, b) == 0
来源：http://uze.zhixingplan.top

[S07] C：数组遍历求和
来源：http://acg.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wax.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://fmu.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://anp.jyoumei.cn

[S09] C：结构体定义与初始化
来源：http://jaw.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lbj.fehbvm.com

[S10] C：指针与解引用
来源：http://ckh.yangfankeji.com

int *p = &a;  *p = 5;
来源：http://smi.gotoacloud.top

[S11] C：逐行读文件
来源：http://tjw.cashguo.top

FILE *f = fopen("a.txt", "r");
来源：http://vgd.shuidangran.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pki.ehwqpu.com

fclose(f);
来源：http://qjl.daxiang520.top

[S12] C：写文件
来源：http://yus.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mpr.cdnleiting.top

[S13] C：宏定义
来源：http://oxj.hammf.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hfk.gaohongyu789.top

[S14] C：枚举
来源：http://zfd.feifeiyinyue.top

enum Color { RED, GREEN, BLUE };
来源：http://aqn.hesvh.cn

[S15] C：类型转换
来源：http://xwn.meibo888.top

(double) a / b
来源：http://kke.zdqjudy.top

[S16] C：位操作置位
来源：http://lfa.sxryk.cn

x |= (1 << 3);
来源：http://xum.fehbvm.com

[S17] C：安全拼接字符串
来源：http://rsh.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lte.zycfv.cn

[S18] C：命令行参数
来源：http://vms.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://yxx.guowangkeji.top

[S19] C：快速排序
来源：http://crw.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://syi.chenzaomai.com

[S20] C：二分查找
来源：http://jhc.jlsjyb.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://eav.zhijiandao.cn

[S21] C：字符类别判断
来源：http://tge.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://exh.yj20258.top

[S22] C：字符串转数字
来源：http://vgv.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fme.redwolf501.top

[S23] C：随机数
来源：http://ege.0kj1m.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://frz.tianlin.xyz

[S24] C：获取本地时间
来源：http://dyc.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://aer.gogol.net.cn

[S25] C：内存拷贝
来源：http://qdk.redwolf501.top

memcpy(dst, src, n);
来源：http://nfn.smart0.xyz

[S26] C：内存清零
来源：http://mrw.52xcode.cn

memset(a, 0, sizeof a);
来源：http://ymq.wangdashe.top

[S27] C：定义常量
来源：http://adu.hywenlv.cn

const double PI = 3.14159;
来源：http://vfy.zycfv.cn

[S28] C：静态变量
来源：http://bzs.jiagoushi.top

static int counter = 0;
来源：http://rgw.yvedp.cn

[S29] C：变参函数
来源：http://etf.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qlt.yuxming.cn

[S30] C：头文件保护
来源：http://yty.andypj.xyz

#ifndef X_H
来源：http://aqh.ivvv.top

#define X_H
来源：http://kcw.xuetiantiany.cn

#endif
来源：http://ddw.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://vni.xylfe.cn

#include <iostream>
来源：http://lny.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://lvm.9152youxi.cn

[S32] C++：字符串
来源：http://lal.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://inm.aizwys.cn


<!-- 参考信息 -->