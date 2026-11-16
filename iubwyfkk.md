代发 wailian999

ROLLBACK TO sp1;
来源：http://tbe.sjlbkw.cn

[Q69] 查看执行计划
来源：http://rmc.zhixingplan.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qfa.jinyuanbaomall.cn

[Q70] 更新统计信息
来源：http://cwr.fzhhl.top

ANALYZE TABLE users;
来源：http://spt.jianghu66.top

[Q71] 查看建表语句
来源：http://unm.sysykeji.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://uwv.shzxlz.cn

[Q72] 查看索引
来源：http://tqv.9152youxi.cn

SHOW INDEX FROM users;
来源：http://ynl.ybcxt.top

[Q73] 查看表状态
来源：http://fze.andypj.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://fme.yj202588.top

[Q74] 强制使用索引
来源：http://nim.zdbjq.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mdv.ppjwa.cn

[Q75] 日期格式化
来源：http://cbl.nwbrower.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ieq.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://toy.mhx1999.top

[Q76] 按天统计
来源：http://hjc.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mtk.sufxvd.cn

[Q77] 时间加减
来源：http://fxk.yj202588.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ffj.hfpthk.cn

[Q78] 当前时间
来源：http://kmy.gogol.net.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rhd.havefunace.top

[Q79] 字符串拼接
来源：http://usj.yj20258888.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lxt.sjlbkw.cn

[Q80] 字符串截取
来源：http://afl.haohaochexian.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://exg.dianchejie.cn

[Q81] 字符串替换
来源：http://xlu.sjlbkw.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://euy.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://gzx.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://eea.c1oappe.top

[Q83] 大小写转换
来源：http://ogm.hongshengwenyu.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sbv.hesvh.cn

[Q84] 去除首尾空格
来源：http://khv.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://bxz.hfpthk.cn

[Q85] 数值取整
来源：http://ejv.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rvm.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://hxs.tianlin.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://tgi.zycfv.cn

[Q87] JSON 字段做条件
来源：http://slb.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gxg.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://uhm.zhixingplan.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nze.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zgj.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://nju.yuanzhike.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uvn.jlsjyb.cn

[Q90] 生成序号列
来源：http://rlr.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jbt.gzhubu.top

================================================================================
来源：http://ytt.gotoacloud.top

R. Bash 专题
来源：http://agm.bjfxy.top

================================================================================
来源：http://tqh.ybcxt.top

[R01] shebang 与严格模式
来源：http://yko.dianchejie.cn

#!/usr/bin/env bash
来源：http://sbi.sweek.top

set -euo pipefail
来源：http://mcc.ivvv.top

[R02] 变量赋值与使用
来源：http://ivf.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://mld.yueranfly.top

[R03] 只读变量
来源：http://kef.havefunace.top

readonly PI=3.14
来源：http://rcs.gogol.net.cn

[R04] 位置参数
来源：http://fxp.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qsa.fengsongda.top

[R05] 参数默认值
来源：http://jro.yangfankeji.com

name="${1:-default}"
来源：http://oku.jiagoushi.top

[R06] 判断命令是否存在
来源：http://zwp.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wwi.ybcxt.top

[R07] if 判断文件
来源：http://xvj.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hoo.wangdashe.top

[R08] 数值比较
来源：http://ria.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://orw.cdnleiting.top

[R09] 字符串比较
来源：http://urk.shzxlz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vro.jinghuilouyu.cn

[R10] 正则匹配
来源：http://nvv.zdbjq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nyl.sweek.top

[R11] case 多分支
来源：http://llw.xylfe.cn

case "$1" in
来源：http://vlm.svipenyu.cn

start) echo "启动" ;;
来源：http://oyk.smart0.xyz

stop)  echo "停止" ;;
来源：http://nzh.yueranfly.top

*)     echo "未知命令" ;;
来源：http://hak.andypj.xyz

esac
来源：http://bzu.nwbrower.top

[R12] for 遍历文件
来源：http://jpw.yfazqb.com

for f in *.txt; do echo "$f"; done
来源：http://pkb.ivvv.top

[R13] for 计数循环
来源：http://grx.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://keu.yangfankeji.com

[R14] C 风格 for
来源：http://yoy.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gpy.c1oappe.top

[R15] while 逐行读文件
来源：http://glz.xingfuxueyuan.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dxo.wangshuangyany.cn

[R16] until 等待条件
来源：http://prg.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nce.zdbjq.cn

[R17] 数组定义与取值
来源：http://xho.smart0.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://kpk.tanke756.top

[R18] 遍历数组
来源：http://uig.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://eyp.nanxuanxn.top

[R19] 数组长度
来源：http://ykk.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://rvg.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://bam.xinyue.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://omw.cdnleiting.top

[R21] 字符串长度
来源：http://nbm.yuxming.cn

echo "${#s}"
来源：http://rjo.zhongyouzk.top

[R22] 截取子串
来源：http://tuc.52xcode.cn

echo "${s:0:5}"
来源：http://psu.wangshuangyany.cn

[R23] 字符串替换
来源：http://pbj.tianlin.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://haw.jinghuilouyu.cn

[R24] 大小写转换
来源：http://hsc.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qqb.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://wwy.gotoacloud.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fhy.birdmap.top

[R26] 命令替换
来源：http://xmz.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://lxo.redwolf501.top

[R27] 算术展开
来源：http://aog.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://bbk.ybcxt.top

[R28] 浮点运算
来源：http://xyu.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://uec.sufxvd.cn

[R29] 定义函数
来源：http://oip.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dhr.cashguo.top

[R30] 函数返回状态码
来源：http://yrw.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://pnn.zhijiandao.cn

[R31] 局部变量
来源：http://udd.ydzc1.top

f() { local x=1; echo "$x"; }
来源：http://unx.cucudq.cn

[R32] 参数个数校验
来源：http://drc.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vzm.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://ctq.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sga.guowangkeji.top

[R34] 退出时清理
来源：http://yar.52xcode.cn

trap 'rm -f "$tmp"' EXIT
来源：http://fvo.snrcjt.cn

[R35] 后台执行并等待
来源：http://ypg.vehdjk.com

sleep 5 & pid=$!; wait "$pid"
来源：http://yld.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://bye.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xmh.cashguo.top

[R37] 把输出赋给变量
来源：http://mja.meibo888.top

files=$(ls -1)
来源：http://hlr.zhengqikj.top

[R38] 管道串联
来源：http://cww.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://ovk.zycfv.cn

[R39] 重定向标准输出与错误
来源：http://xlo.xinyue.icu

cmd > out.log 2>&1
来源：http://yod.hcnkem.com

[R40] 追加写日志
来源：http://vpr.feifeiyinyue.top

echo "log" >> out.log
来源：http://wmh.ehwqpu.com

[R41] 丢弃输出
来源：http://lnu.xylfe.cn

cmd >/dev/null 2>&1
来源：http://afx.bjfxy.top

[R42] 输入重定向
来源：http://eun.hnxiangtu.top

wc -l < a.txt
来源：http://myb.cdnleiting.top

[R43] 按名字查找文件
来源：http://anp.nanxuanxn.top

find . -name "*.log" -type f
来源：http://epu.yuanzhike.top

[R44] 按修改时间查找
来源：http://dns.yangfankeji.com

find . -mtime -7 -type f
来源：http://ixc.cdnleiting.top

[R45] 批量删除
来源：http://ixj.9152youxi.cn

find . -name "*.tmp" -delete
来源：http://vqo.xziqi.cn

[R46] 递归替换文件内容
来源：http://lvh.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://utt.jqgfzy.top

[R47] sed 单行替换
来源：http://kqg.jinqigufen.top

sed -i 's/foo/bar/g' a.txt
来源：http://wdf.xuetiantiany.cn

[R48] awk 取指定列
来源：http://pyf.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://sbb.pycfn.com

[R49] awk 带条件
来源：http://mto.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nnp.yangfankeji.com

[R50] awk 求和
来源：http://lpi.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://qcx.aizwys.cn

[R51] 排序去重取前几
来源：http://ohw.nanxuanxn.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gal.mhx1999.top

[R52] 统计行数
来源：http://jew.nanxuanxn.top

wc -l a.txt
来源：http://npp.chenzaomai.com

[R53] 查看文件头与实时尾
来源：http://qoc.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zvq.nwbrower.top

[R54] 比较两个文件
来源：http://rqz.yfazqb.com

diff a.txt b.txt
来源：http://nsl.zdbjq.cn

[R55] 压缩与解压
来源：http://jmr.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vyk.tanke756.top

[R56] 远程拷贝
来源：http://qpv.xuetiantiany.cn

scp file user@host:/path/
来源：http://aqm.feifeiyinyue.top

[R57] 远程执行命令
来源：http://awb.zhijiandao.cn

ssh user@host 'uptime'
来源：http://xvb.pycfn.com

[R58] 下载文件
来源：http://tqg.dashuyun.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zqy.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://fsn.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vja.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://bwx.fktsv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xlx.yfazqb.com

[R61] 磁盘占用
来源：http://xda.ydjk.org.cn

df -h;  du -sh *
来源：http://qox.pycfn.com

[R62] 找最占空间的文件
来源：http://hdx.ybcxt.top

du -ah . | sort -rh | head -10
来源：http://bvl.chenjidiqi.icu

[R63] 内存与进程
来源：http://jub.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://qrm.zhoulong.xyz

[R64] 结束进程
来源：http://qfz.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://qhm.yonumen.top

[R65] 查看端口占用
来源：http://igc.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkh.aibaodan.cn

[R66] 定时任务
来源：http://cks.52xcode.cn

crontab -e;  crontab -l
来源：http://dwd.zhaomingkeji.xyz

[R67] 生成随机十六进制串
来源：http://rwb.jyoumei.cn

openssl rand -hex 16
来源：http://xeb.yuxming.cn

[R68] 计算文件校验值
来源：http://pmi.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://slm.daria6918.cn

[R69] 生成随机密码
来源：http://sod.nanxuanxn.top

head -c 16 /dev/urandom | base64
来源：http://wwe.cheryme.top

[R70] 时间戳与互转
来源：http://dhj.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://npf.yuanzhike.top

[R71] 日期格式化
来源：http://zla.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://zzh.guowangkeji.top

[R72] 等待端口就绪
来源：http://jok.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fiq.smart0.xyz

[R73] 分割大日志
来源：http://ssf.shzxlz.cn

split -l 1000 big.log part_
来源：http://ldf.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://trp.kuanghao11.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mfx.xuetiantiany.cn

[R75] 导出环境变量
来源：http://xrd.316326.xyz

export PATH="$HOME/bin:$PATH"
来源：http://kdm.chenlongwang.top

[R76] 使用临时文件
来源：http://wvu.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uoj.shangyingyoupin.top

[R77] 读取用户输入
来源：http://idc.sweek.top

read -rp "请输入: " ans
来源：http://kds.jianghu66.top

[R78] 交互式菜单
来源：http://icr.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://shq.cqqwz.cn

[R79] 解析命令行选项
来源：http://hbv.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wsm.birdmap.top

[R80] 查看脚本执行耗时
来源：http://xuf.ivvv.top

time ./run.sh
来源：http://oym.gzhubu.top

================================================================================
来源：http://xei.gogol.net.cn

S. C / C++ 专题
来源：http://bom.hongshengwenyu.top

================================================================================
来源：http://snq.gotoacloud.top

[S01] C：Hello World
来源：http://htu.sjlbkw.cn

#include <stdio.h>
来源：http://zue.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aes.fzhhl.top

[S02] C：变量与格式化输出
来源：http://ser.cucudq.cn

int a = 10; printf("%d\n", a);
来源：http://spx.cashguo.top

[S03] C：读入整数
来源：http://kbo.jiagoushi.top

int x; scanf("%d", &x);
来源：http://xbm.wangshuangyany.cn

[S04] C：字符串复制
来源：http://ftx.aibaodan.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lya.bjfxy.top

[S05] C：字符串长度
来源：http://jud.cucudq.cn

strlen(s)
来源：http://ijx.9152youxi.cn

[S06] C：字符串比较
来源：http://omt.cashguo.top

strcmp(a, b) == 0
来源：http://hxw.hnxiangtu.top

[S07] C：数组遍历求和
来源：http://nap.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wox.cqqwz.cn

[S08] C：动态内存分配与释放
来源：http://rlw.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kep.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://klf.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hfa.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://ded.c1oappe.top

int *p = &a;  *p = 5;
来源：http://hlc.jinqigfzy.top

[S11] C：逐行读文件
来源：http://eif.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://upo.cashguo.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zhf.jinqigfzy.top

fclose(f);
来源：http://nbr.jlsjyb.cn

[S12] C：写文件
来源：http://szz.bbcook.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yoy.jqgufenzy.top

[S13] C：宏定义
来源：http://ddf.hfpthk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://coh.fehbvm.com

[S14] C：枚举
来源：http://imb.ppjwa.cn

enum Color { RED, GREEN, BLUE };
来源：http://tdh.haohaochexian.top

[S15] C：类型转换
来源：http://gkn.jinqigufen.top

(double) a / b
来源：http://mnh.sufxvd.cn

[S16] C：位操作置位
来源：http://try.gogol.net.cn

x |= (1 << 3);
来源：http://wzl.ydjk.org.cn

[S17] C：安全拼接字符串
来源：http://awb.shanyushiyangtech.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dga.dashuyun.cn

[S18] C：命令行参数
来源：http://iiu.ydjk.org.cn

int main(int argc, char **argv)
来源：http://gyd.sufxvd.cn

[S19] C：快速排序
来源：http://gsa.ctjpmb.com

qsort(a, n, sizeof(int), cmp);
来源：http://mxs.chenzaomai.com

[S20] C：二分查找
来源：http://ndy.nanxinkj.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://crz.xuetiantiany.cn

[S21] C：字符类别判断
来源：http://zpr.yj20258888.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rjv.haohaochexian.top

[S22] C：字符串转数字
来源：http://vbg.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nky.gotoacloud.top

[S23] C：随机数
来源：http://kjt.nanxuanxn.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nkm.jinqigufen.top

[S24] C：获取本地时间
来源：http://xdf.dashuyun.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ycq.tianlin.xyz

[S25] C：内存拷贝
来源：http://kcu.hywenlv.cn

memcpy(dst, src, n);
来源：http://hjt.chenjidiqi.icu

[S26] C：内存清零
来源：http://rot.zdqjudy.top

memset(a, 0, sizeof a);
来源：http://dkl.hnqzz.top

[S27] C：定义常量
来源：http://pfk.cdnleiting.top

const double PI = 3.14159;
来源：http://qmo.snrcjt.cn

[S28] C：静态变量
来源：http://gnf.tanke756.top

static int counter = 0;
来源：http://ntq.haohaochexian.top

[S29] C：变参函数
来源：http://glk.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dbv.yangfankeji.com

[S30] C：头文件保护
来源：http://uqc.yfazqb.com

#ifndef X_H
来源：http://obj.cucudq.cn

#define X_H
来源：http://jjo.tian-w.cn

#endif
来源：http://pxa.redwolf501.top

[S31] C++：Hello World
来源：http://wfa.dashuyun.cn

#include <iostream>
来源：http://xyu.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://riu.jqgfzy.top

[S32] C++：字符串
来源：http://bhs.gogol.net.cn

std::string s = "hi";  s += "!";
来源：http://cfs.chenlongwang.top

[S33] C++：vector 增删
来源：http://wba.hnqzz.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zom.daxiang520.top

[S34] C++：遍历 vector
来源：http://nkc.cqqwz.cn

for (auto &x : v) { std::cout << x; }
来源：http://lxa.ivvv.top

[S35] C++：map
来源：http://sbk.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xnu.sufxvd.cn

[S36] C++：unordered_map
来源：http://uju.sxryk.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yce.daxiang520.top

[S37] C++：set
来源：http://cyd.sjlbkw.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jju.xuetiantiany.cn

[S38] C++：排序
来源：http://lip.sxryk.cn

std::sort(v.begin(), v.end());
来源：http://oad.daria6918.cn


<!-- 参考信息 -->