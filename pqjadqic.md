代发 wailian999

SHOW INDEX FROM users;
来源：http://vog.hongshengwenyu.top

[Q73] 查看表状态
来源：http://ugo.xylfe.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kda.birdmap.top

[Q74] 强制使用索引
来源：http://fgd.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bfm.cheryme.top

[Q75] 日期格式化
来源：http://leb.yj202588.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fha.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://zee.yuxming.cn

[Q76] 按天统计
来源：http://cka.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kvc.hammf.cn

[Q77] 时间加减
来源：http://chs.xziqi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wnr.gaohongyu789.top

[Q78] 当前时间
来源：http://veo.jiagoushi.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qyc.havefunace.top

[Q79] 字符串拼接
来源：http://ohv.nanxinkj.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hnx.jianghu66.top

[Q80] 字符串截取
来源：http://vye.hnxiangtu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://fxz.zhijiandao.cn

[Q81] 字符串替换
来源：http://idx.hywenlv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ean.havefunace.top

[Q82] 字符长度与字节长度
来源：http://xjq.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pzi.tanke756.top

[Q83] 大小写转换
来源：http://xax.nanxinkj.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://xjn.hongshengwenyu.top

[Q84] 去除首尾空格
来源：http://uni.guowangkeji.top

SELECT TRIM(name) FROM users;
来源：http://zxf.guannengcc.top

[Q85] 数值取整
来源：http://jps.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://phx.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://uqt.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zeh.tanke756.top

[Q87] JSON 字段做条件
来源：http://tob.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrm.tianlin.xyz

[Q88] 行转列（条件聚合）
来源：http://gme.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://edp.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://aar.316326.xyz

[Q89] 判断表是否存在
来源：http://rit.zhongyouzk.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vcv.cucudq.cn

[Q90] 生成序号列
来源：http://nef.svipenyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kzo.zhaomingkeji.xyz

================================================================================
来源：http://wck.xingfuxueyuan.xyz

R. Bash 专题
来源：http://ivc.yuxming.cn

================================================================================
来源：http://sfo.birdmap.top

[R01] shebang 与严格模式
来源：http://fhv.bjfxy.top

#!/usr/bin/env bash
来源：http://dsk.0kj1m.cn

set -euo pipefail
来源：http://oak.yongpay.top

[R02] 变量赋值与使用
来源：http://cpw.ctjpmb.com

name="Tom"; echo "$name"
来源：http://gfk.zhoulong.xyz

[R03] 只读变量
来源：http://xvf.zdbjq.cn

readonly PI=3.14
来源：http://gaf.snrcjt.cn

[R04] 位置参数
来源：http://tze.andypj.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ktl.ydzc1.top

[R05] 参数默认值
来源：http://grw.smart0.xyz

name="${1:-default}"
来源：http://ovs.vehdjk.com

[R06] 判断命令是否存在
来源：http://vlv.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pkd.sxryk.cn

[R07] if 判断文件
来源：http://mox.cheryme.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jjx.chenlongwang.top

[R08] 数值比较
来源：http://fof.cucudq.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://nuc.ydjk.org.cn

[R09] 字符串比较
来源：http://yya.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://rlk.hfpthk.cn

[R10] 正则匹配
来源：http://hri.hysaishi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hsu.hysaishi.cn

[R11] case 多分支
来源：http://rdl.quarkkingdee.top

case "$1" in
来源：http://oxe.shangyingyoupin.top

start) echo "启动" ;;
来源：http://mqp.yfazqb.com

stop)  echo "停止" ;;
来源：http://mme.sysykeji.top

*)     echo "未知命令" ;;
来源：http://eua.pycfn.com

esac
来源：http://rqc.9152youxi.cn

[R12] for 遍历文件
来源：http://tvn.fktsv.cn

for f in *.txt; do echo "$f"; done
来源：http://wby.hammf.cn

[R13] for 计数循环
来源：http://poy.svipenyu.cn

for i in {1..10}; do echo "$i"; done
来源：http://mgf.yangfankeji.com

[R14] C 风格 for
来源：http://txj.dianchejie.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jkc.dianchejie.cn

[R15] while 逐行读文件
来源：http://enk.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xvw.jinqigufen.top

[R16] until 等待条件
来源：http://ouy.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://enp.daxiang520.top

[R17] 数组定义与取值
来源：http://eti.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mej.yj20258888.top

[R18] 遍历数组
来源：http://enk.hfpthk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://smg.hfpthk.cn

[R19] 数组长度
来源：http://cby.vqdsnc.cn

echo "${#arr[@]}"
来源：http://nzf.aizwys.cn

[R20] 关联数组（字典）
来源：http://zgy.guannengcc.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bxt.chenjidiqi.icu

[R21] 字符串长度
来源：http://did.zdqjudy.top

echo "${#s}"
来源：http://hmk.ydjk.org.cn

[R22] 截取子串
来源：http://bln.ppjwa.cn

echo "${s:0:5}"
来源：http://lih.epnwcf.com

[R23] 字符串替换
来源：http://dpo.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rpy.uphjek.com

[R24] 大小写转换
来源：http://cpt.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hdx.chenlongwang.top

[R25] 去后缀 / 去前缀
来源：http://xfp.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://jkj.sufxvd.cn

[R26] 命令替换
来源：http://lkq.yonumen.top

now=$(date +%F); echo "$now"
来源：http://qfh.yangfankeji.com

[R27] 算术展开
来源：http://gsx.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://vlm.bbcook.cn

[R28] 浮点运算
来源：http://mhp.yvedp.cn

echo "scale=2; 10/3" | bc
来源：http://zgk.hysaishi.cn

[R29] 定义函数
来源：http://tgv.fzhhl.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cgo.fktsv.cn

[R30] 函数返回状态码
来源：http://iaa.zhaomingkeji.xyz

f() { return 0; }; f || echo "失败了"
来源：http://vcm.yuxming.cn

[R31] 局部变量
来源：http://smv.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://rto.hongshengwenyu.top

[R32] 参数个数校验
来源：http://fus.ppjwa.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kew.hesvh.cn

[R33] 捕获错误并提示行号
来源：http://hby.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lgp.guowangkeji.top

[R34] 退出时清理
来源：http://myt.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://jig.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://oxb.vqdsnc.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sty.gotoacloud.top

[R36] 并发执行多个任务
来源：http://tlc.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cft.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://slk.uphjek.com

files=$(ls -1)
来源：http://afq.smart0.xyz

[R38] 管道串联
来源：http://liu.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://dfk.316326.xyz

[R39] 重定向标准输出与错误
来源：http://kxi.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://rds.jqgfzy.top

[R40] 追加写日志
来源：http://qua.nwbrower.top

echo "log" >> out.log
来源：http://uiu.jinghuilouyu.cn

[R41] 丢弃输出
来源：http://jvv.ehwqpu.com

cmd >/dev/null 2>&1
来源：http://xia.bbcook.cn

[R42] 输入重定向
来源：http://jsi.birdmap.top

wc -l < a.txt
来源：http://ibl.haohaochexian.top

[R43] 按名字查找文件
来源：http://pil.0kj1m.cn

find . -name "*.log" -type f
来源：http://ksl.guannengcc.top

[R44] 按修改时间查找
来源：http://pdm.zhijiandao.cn

find . -mtime -7 -type f
来源：http://jph.bjfxy.top

[R45] 批量删除
来源：http://gsa.hesvh.cn

find . -name "*.tmp" -delete
来源：http://yrh.havefunace.top

[R46] 递归替换文件内容
来源：http://vqo.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mdw.hesvh.cn

[R47] sed 单行替换
来源：http://ere.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://sbc.9152youxi.cn

[R48] awk 取指定列
来源：http://xar.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://tjz.smart0.xyz

[R49] awk 带条件
来源：http://afj.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ref.meibo888.top

[R50] awk 求和
来源：http://oht.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://vaz.quarkkingdee.top

[R51] 排序去重取前几
来源：http://mkv.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://bfq.andypj.xyz

[R52] 统计行数
来源：http://nqs.yfazqb.com

wc -l a.txt
来源：http://mjq.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://ezz.pengpengdd.cyou

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fil.kuanghao11.cn

[R54] 比较两个文件
来源：http://hvn.yvedp.cn

diff a.txt b.txt
来源：http://jjw.ybcxt.top

[R55] 压缩与解压
来源：http://bdy.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://tuy.wangdashe.top

[R56] 远程拷贝
来源：http://ggb.shzxlz.cn

scp file user@host:/path/
来源：http://bwq.316326.xyz

[R57] 远程执行命令
来源：http://zkb.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://dul.shanyushiyangtech.top

[R58] 下载文件
来源：http://mux.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bjo.yfazqb.com

[R59] 发 POST JSON
来源：http://hxa.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jiv.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://fkj.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ljx.aizwys.cn

[R61] 磁盘占用
来源：http://tba.ywan-chungtsiang.top

df -h;  du -sh *
来源：http://sqr.zhengqikj.top

[R62] 找最占空间的文件
来源：http://hhn.pycfn.com

du -ah . | sort -rh | head -10
来源：http://ipw.sjlbkw.cn

[R63] 内存与进程
来源：http://zap.jiagoushi.top

free -h;  ps aux | grep nginx
来源：http://puu.meibo888.top

[R64] 结束进程
来源：http://qgf.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://ocl.iojbl.cn

[R65] 查看端口占用
来源：http://ygd.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ruv.tian-w.cn

[R66] 定时任务
来源：http://jla.yj202588.top

crontab -e;  crontab -l
来源：http://wef.kuanghao11.cn

[R67] 生成随机十六进制串
来源：http://tub.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://lou.cqqwz.cn

[R68] 计算文件校验值
来源：http://hwh.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zse.pengpengdd.cyou

[R69] 生成随机密码
来源：http://cae.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://dxe.yangfankeji.com

[R70] 时间戳与互转
来源：http://oyw.shzxlz.cn

date +%s;  date -d @1700000000
来源：http://fmh.kuanghao11.cn

[R71] 日期格式化
来源：http://oor.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://rjq.yanxiufei.cn

[R72] 等待端口就绪
来源：http://hmv.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yku.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://tue.zhijiandao.cn

split -l 1000 big.log part_
来源：http://uby.xingfuxueyuan.xyz

[R74] 批量重命名
来源：http://nfv.cheryme.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ovb.zhongyouzk.top

[R75] 导出环境变量
来源：http://ksc.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://qnz.hfpthk.cn

[R76] 使用临时文件
来源：http://cht.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qqf.iojbl.cn

[R77] 读取用户输入
来源：http://bhn.vqdsnc.cn

read -rp "请输入: " ans
来源：http://eyw.sysykeji.top

[R78] 交互式菜单
来源：http://yoa.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gxp.sysykeji.top

[R79] 解析命令行选项
来源：http://njh.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wah.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://apc.wangshuangyany.cn

time ./run.sh
来源：http://kgd.hfpthk.cn

================================================================================
来源：http://mnv.xinyue.icu

S. C / C++ 专题
来源：http://reu.zhengqikj.top

================================================================================
来源：http://knk.ydzc1.top

[S01] C：Hello World
来源：http://sbs.ppjwa.cn

#include <stdio.h>
来源：http://tku.feifeiyinyue.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vcj.sufxvd.cn

[S02] C：变量与格式化输出
来源：http://djq.zhoulong.xyz

int a = 10; printf("%d\n", a);
来源：http://voj.aibaodan.cn

[S03] C：读入整数
来源：http://lhh.xinyue.icu

int x; scanf("%d", &x);
来源：http://xuq.hammf.cn

[S04] C：字符串复制
来源：http://xwl.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://exi.chenjidiqi.icu

[S05] C：字符串长度
来源：http://vpz.tian-w.cn

strlen(s)
来源：http://ohf.pengpengdd.cyou

[S06] C：字符串比较
来源：http://mxu.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://vff.ppjwa.cn

[S07] C：数组遍历求和
来源：http://klf.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eek.pycfn.com

[S08] C：动态内存分配与释放
来源：http://kpa.yanxiufei.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://noz.chenzaomai.com

[S09] C：结构体定义与初始化
来源：http://fgy.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zca.xinyue.icu

[S10] C：指针与解引用
来源：http://ser.tian-w.cn

int *p = &a;  *p = 5;
来源：http://vlz.mhx1999.top

[S11] C：逐行读文件
来源：http://gsq.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://sus.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://jpv.chenjidiqi.icu

fclose(f);
来源：http://nez.nanxuanxn.top

[S12] C：写文件
来源：http://eks.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://imi.jlsjyb.cn

[S13] C：宏定义
来源：http://fjt.haohaochexian.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xnk.haohaochexian.top

[S14] C：枚举
来源：http://anl.smart0.xyz

enum Color { RED, GREEN, BLUE };
来源：http://mrd.c1oappe.top

[S15] C：类型转换
来源：http://pfm.ydzc1.top

(double) a / b
来源：http://oga.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://wfs.redwolf501.top

x |= (1 << 3);
来源：http://lvt.sufxvd.cn

[S17] C：安全拼接字符串
来源：http://tsv.yfazqb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gnp.quarkkingdee.top

[S18] C：命令行参数
来源：http://nnh.jyoumei.cn

int main(int argc, char **argv)
来源：http://rpo.zhengqikj.top

[S19] C：快速排序
来源：http://ygf.xinyue.icu

qsort(a, n, sizeof(int), cmp);
来源：http://uyh.nanxinkj.top

[S20] C：二分查找
来源：http://xdo.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ory.gaohongyu789.top

[S21] C：字符类别判断
来源：http://cny.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sxj.yj202588.top

[S22] C：字符串转数字
来源：http://pno.chenlongwang.top

atoi("42");  strtod("3.14", NULL);
来源：http://wym.sjlbkw.cn

[S23] C：随机数
来源：http://qkg.redwolf501.top

srand(time(NULL));  int r = rand() % 100;
来源：http://qcl.jiagoushi.top

[S24] C：获取本地时间
来源：http://bmp.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ijc.ppjwa.cn

[S25] C：内存拷贝
来源：http://vka.hcnkem.com

memcpy(dst, src, n);
来源：http://oft.kuanghao11.cn

[S26] C：内存清零
来源：http://aan.jinyuanbaomall.cn

memset(a, 0, sizeof a);
来源：http://lpy.daxiang520.top

[S27] C：定义常量
来源：http://ncu.guowangkeji.top

const double PI = 3.14159;
来源：http://hgv.havefunace.top

[S28] C：静态变量
来源：http://ahp.zdqjudy.top

static int counter = 0;
来源：http://lht.ehwqpu.com

[S29] C：变参函数
来源：http://uac.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rhs.hysaishi.cn

[S30] C：头文件保护
来源：http://ohg.tarul.cn

#ifndef X_H
来源：http://slf.tanke756.top

#define X_H
来源：http://dob.ydjk.org.cn

#endif
来源：http://jrh.gotoacloud.top

[S31] C++：Hello World
来源：http://rog.zdqjudy.top

#include <iostream>
来源：http://mlk.yuanzhike.top

int main() { std::cout << "Hello\n"; }
来源：http://qkm.zhaomingkeji.xyz

[S32] C++：字符串
来源：http://bdk.yangfankeji.com

std::string s = "hi";  s += "!";
来源：http://drx.fengsongda.top

[S33] C++：vector 增删
来源：http://kzy.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ffn.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://knm.redwolf501.top

for (auto &x : v) { std::cout << x; }
来源：http://wpl.aizwys.cn

[S35] C++：map
来源：http://zfr.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vmn.nanxinkj.top

[S36] C++：unordered_map
来源：http://ywn.yueranfly.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://aqt.ppjwa.cn

[S37] C++：set
来源：http://zsq.snrcjt.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kqb.nanxinkj.top

[S38] C++：排序
来源：http://awr.daria6918.cn

std::sort(v.begin(), v.end());
来源：http://xpx.jinqigfzy.top

[S39] C++：自定义比较器排序
来源：http://wbv.hcnkem.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ufc.jiagoushi.top

[S40] C++：查找元素
来源：http://tfo.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ezl.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://ked.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ayb.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://czb.gogol.net.cn

class B : public Base { public: void f() override {} };
来源：http://mfi.jinyuanbaomall.cn


<!-- 参考信息 -->