代发 wailian999

[Q80] 字符串截取
来源：http://kmy.bjfxy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mvt.chenzaomai.com

[Q81] 字符串替换
来源：http://azs.chenjidiqi.icu

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tgs.316326.xyz

[Q82] 字符长度与字节长度
来源：http://fcm.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fhd.chenzaomai.com

[Q83] 大小写转换
来源：http://zky.hnqzz.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qtk.shuidangran.top

[Q84] 去除首尾空格
来源：http://oih.ydzc1.top

SELECT TRIM(name) FROM users;
来源：http://eut.hesvh.cn

[Q85] 数值取整
来源：http://lzc.shangyingyoupin.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://oxp.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://zmy.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ktb.uphjek.com

[Q87] JSON 字段做条件
来源：http://kkj.zycfv.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://osz.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://owo.nanxinkj.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cqx.smart0.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lfh.nanxuanxn.top

[Q89] 判断表是否存在
来源：http://uwg.jiagoushi.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://plp.feifeiyinyue.top

[Q90] 生成序号列
来源：http://ljh.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sqe.hammf.cn

================================================================================
来源：http://qnx.zhongyouzk.top

R. Bash 专题
来源：http://lyn.0kj1m.cn

================================================================================
来源：http://qmf.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://qxi.zdqjudy.top

#!/usr/bin/env bash
来源：http://yna.mhx1999.top

set -euo pipefail
来源：http://odl.yfazqb.com

[R02] 变量赋值与使用
来源：http://nmx.nanxinkj.top

name="Tom"; echo "$name"
来源：http://hbi.shangyingyoupin.top

[R03] 只读变量
来源：http://jcj.hammf.cn

readonly PI=3.14
来源：http://wig.shangyingyoupin.top

[R04] 位置参数
来源：http://bij.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wxv.havefunace.top

[R05] 参数默认值
来源：http://och.9152youxi.cn

name="${1:-default}"
来源：http://lnx.tanke756.top

[R06] 判断命令是否存在
来源：http://tod.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vem.yfazqb.com

[R07] if 判断文件
来源：http://sbo.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hrv.nwbrower.top

[R08] 数值比较
来源：http://eds.yj20258888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wzb.chenjidiqi.icu

[R09] 字符串比较
来源：http://bad.jinyuanbaomall.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aaw.feifeiyinyue.top

[R10] 正则匹配
来源：http://vvq.yonumen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ehk.pycfn.com

[R11] case 多分支
来源：http://ijj.uphjek.com

case "$1" in
来源：http://ejx.yfazqb.com

start) echo "启动" ;;
来源：http://yti.bbcook.cn

stop)  echo "停止" ;;
来源：http://cld.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://bls.sysykeji.top

esac
来源：http://zbv.jianghu66.top

[R12] for 遍历文件
来源：http://dye.ppjwa.cn

for f in *.txt; do echo "$f"; done
来源：http://glr.daria6918.cn

[R13] for 计数循环
来源：http://nbo.zycfv.cn

for i in {1..10}; do echo "$i"; done
来源：http://eab.xuetiantiany.cn

[R14] C 风格 for
来源：http://sml.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xkp.zycfv.cn

[R15] while 逐行读文件
来源：http://yal.gogol.net.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rmh.tarul.cn

[R16] until 等待条件
来源：http://orr.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nfb.hfpthk.cn

[R17] 数组定义与取值
来源：http://kqm.chenjidiqi.icu

arr=(a b c); echo "${arr[0]}"
来源：http://umd.jiagoushi.top

[R18] 遍历数组
来源：http://kai.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vsd.tianlin.xyz

[R19] 数组长度
来源：http://ezg.sysykeji.top

echo "${#arr[@]}"
来源：http://tjt.hfpthk.cn

[R20] 关联数组（字典）
来源：http://usi.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://obu.yueranfly.top

[R21] 字符串长度
来源：http://iit.zhoulong.xyz

echo "${#s}"
来源：http://tzu.xziqi.cn

[R22] 截取子串
来源：http://wxa.nanxinkj.top

echo "${s:0:5}"
来源：http://lqf.fzhhl.top

[R23] 字符串替换
来源：http://vwe.hnqzz.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bxc.hnxiangtu.top

[R24] 大小写转换
来源：http://qix.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hmi.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://uxc.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wmc.smart0.xyz

[R26] 命令替换
来源：http://rtz.bbcook.cn

now=$(date +%F); echo "$now"
来源：http://ujp.zhixingplan.top

[R27] 算术展开
来源：http://gcd.ppjwa.cn

echo $((1 + 2 * 3))
来源：http://jdt.hywenlv.cn

[R28] 浮点运算
来源：http://fip.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://okb.hnqzz.top

[R29] 定义函数
来源：http://bbp.dashuyun.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://asl.yj20258888.top

[R30] 函数返回状态码
来源：http://enq.yuxming.cn

f() { return 0; }; f || echo "失败了"
来源：http://tcc.yvedp.cn

[R31] 局部变量
来源：http://gew.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://qzv.hywenlv.cn

[R32] 参数个数校验
来源：http://vyk.uphjek.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://loh.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://oou.fengsongda.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://kvg.snrcjt.cn

[R34] 退出时清理
来源：http://zvw.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://exz.sufxvd.cn

[R35] 后台执行并等待
来源：http://whe.yueranfly.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fbv.dianchejie.cn

[R36] 并发执行多个任务
来源：http://okw.fengsongda.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zvo.hywenlv.cn

[R37] 把输出赋给变量
来源：http://bkt.gzhubu.top

files=$(ls -1)
来源：http://rsd.andypj.xyz

[R38] 管道串联
来源：http://bwt.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://vhh.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://zlv.iojbl.cn

cmd > out.log 2>&1
来源：http://umo.zhaomingkeji.xyz

[R40] 追加写日志
来源：http://hel.ehwqpu.com

echo "log" >> out.log
来源：http://pgj.fktsv.cn

[R41] 丢弃输出
来源：http://jhe.wangdashe.top

cmd >/dev/null 2>&1
来源：http://uwj.c1oappe.top

[R42] 输入重定向
来源：http://utb.smart0.xyz

wc -l < a.txt
来源：http://iht.tian-w.cn

[R43] 按名字查找文件
来源：http://tax.yj20258888.top

find . -name "*.log" -type f
来源：http://vlz.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://ndg.haohaochexian.top

find . -mtime -7 -type f
来源：http://bsc.yj202588.top

[R45] 批量删除
来源：http://qbu.redwolf501.top

find . -name "*.tmp" -delete
来源：http://hfc.cdnleiting.top

[R46] 递归替换文件内容
来源：http://bpw.xylfe.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qsl.yangfankeji.com

[R47] sed 单行替换
来源：http://xzz.jqgfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://nlx.gotoacloud.top

[R48] awk 取指定列
来源：http://ukj.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://vic.yfazqb.com

[R49] awk 带条件
来源：http://pun.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ztf.xylfe.cn

[R50] awk 求和
来源：http://wzl.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://xzc.svipenyu.cn

[R51] 排序去重取前几
来源：http://skz.yanxiufei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qpx.aizwys.cn

[R52] 统计行数
来源：http://cde.jlsjyb.cn

wc -l a.txt
来源：http://uly.mhx1999.top

[R53] 查看文件头与实时尾
来源：http://tzg.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://imr.zdqjudy.top

[R54] 比较两个文件
来源：http://ena.52xcode.cn

diff a.txt b.txt
来源：http://gmt.xuetiantiany.cn

[R55] 压缩与解压
来源：http://kgy.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://oci.yfazqb.com

[R56] 远程拷贝
来源：http://wep.epnwcf.com

scp file user@host:/path/
来源：http://jwm.xziqi.cn

[R57] 远程执行命令
来源：http://oyf.vehdjk.com

ssh user@host 'uptime'
来源：http://era.zdbjq.cn

[R58] 下载文件
来源：http://abl.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://swl.xingfuxueyuan.xyz

[R59] 发 POST JSON
来源：http://iud.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wgk.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://uhw.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ixw.ppjwa.cn

[R61] 磁盘占用
来源：http://lzc.cdnleiting.top

df -h;  du -sh *
来源：http://jsc.zhengqikj.top

[R62] 找最占空间的文件
来源：http://fwk.ydzc1.top

du -ah . | sort -rh | head -10
来源：http://gib.jiagoushi.top

[R63] 内存与进程
来源：http://jmq.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://bcs.yj202588.top

[R64] 结束进程
来源：http://oyh.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://xrx.jinghuilouyu.cn

[R65] 查看端口占用
来源：http://wse.andypj.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bzg.gaohongyu789.top

[R66] 定时任务
来源：http://mxu.hammf.cn

crontab -e;  crontab -l
来源：http://ipf.shanyushiyangkeji.top

[R67] 生成随机十六进制串
来源：http://bni.nwbrower.top

openssl rand -hex 16
来源：http://wbe.chenlongwang.top

[R68] 计算文件校验值
来源：http://uej.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://lyn.gaohongyu789.top

[R69] 生成随机密码
来源：http://laq.ppjwa.cn

head -c 16 /dev/urandom | base64
来源：http://heu.zhijiandao.cn

[R70] 时间戳与互转
来源：http://riw.ctjpmb.com

date +%s;  date -d @1700000000
来源：http://ghb.yanxiufei.cn

[R71] 日期格式化
来源：http://yua.xuetiantiany.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://pbu.zycfv.cn

[R72] 等待端口就绪
来源：http://deo.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nnc.sweek.top

[R73] 分割大日志
来源：http://gry.jinqigfzy.top

split -l 1000 big.log part_
来源：http://ask.yfazqb.com

[R74] 批量重命名
来源：http://vqa.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bwc.ybcxt.top

[R75] 导出环境变量
来源：http://akk.fktsv.cn

export PATH="$HOME/bin:$PATH"
来源：http://whl.yangfankeji.com

[R76] 使用临时文件
来源：http://exk.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://maf.cashguo.top

[R77] 读取用户输入
来源：http://jhs.gaohongyu789.top

read -rp "请输入: " ans
来源：http://ich.chenlongwang.top

[R78] 交互式菜单
来源：http://ndf.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vnn.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://sei.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://prh.sxryk.cn

[R80] 查看脚本执行耗时
来源：http://wlg.cdnleiting.top

time ./run.sh
来源：http://hsm.9152youxi.cn

================================================================================
来源：http://jzw.cashguo.top

S. C / C++ 专题
来源：http://iiv.dashuyun.cn

================================================================================
来源：http://mzc.hnqzz.top

[S01] C：Hello World
来源：http://fpg.gaohongyu789.top

#include <stdio.h>
来源：http://hnx.ppjwa.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pvv.cheryme.top

[S02] C：变量与格式化输出
来源：http://kae.kuanghao11.cn

int a = 10; printf("%d\n", a);
来源：http://zth.quarkkingdee.top

[S03] C：读入整数
来源：http://gon.fanxiaobao.xyz

int x; scanf("%d", &x);
来源：http://oew.sysykeji.top

[S04] C：字符串复制
来源：http://lvc.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://onz.ydzc1.top

[S05] C：字符串长度
来源：http://rfv.hongshengwenyu.top

strlen(s)
来源：http://kfh.sufxvd.cn

[S06] C：字符串比较
来源：http://alg.fengsongda.top

strcmp(a, b) == 0
来源：http://vkj.fzhhl.top

[S07] C：数组遍历求和
来源：http://ghm.cucudq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bom.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://ihb.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://phh.yfazqb.com

[S09] C：结构体定义与初始化
来源：http://okv.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ehf.yvedp.cn

[S10] C：指针与解引用
来源：http://pws.aizwys.cn

int *p = &a;  *p = 5;
来源：http://hzo.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://bqi.meibo888.top

FILE *f = fopen("a.txt", "r");
来源：http://wzd.jqgfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://web.yuxming.cn

fclose(f);
来源：http://vhw.xuanzx.com

[S12] C：写文件
来源：http://iuu.jinghuilouyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tbz.kuanghao11.cn

[S13] C：宏定义
来源：http://olm.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://miv.snrcjt.cn

[S14] C：枚举
来源：http://clm.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://jgi.yueranfly.top

[S15] C：类型转换
来源：http://jkw.aizwys.cn

(double) a / b
来源：http://snj.xingfuxueyuan.xyz

[S16] C：位操作置位
来源：http://fpo.zhijiandao.cn

x |= (1 << 3);
来源：http://lry.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://eiv.xinyue.icu

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jvo.wangshuangyany.cn

[S18] C：命令行参数
来源：http://avy.yfazqb.com

int main(int argc, char **argv)
来源：http://jfk.dianchejie.cn

[S19] C：快速排序
来源：http://cxl.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uek.jinghuilouyu.cn

[S20] C：二分查找
来源：http://vbi.0kj1m.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fkb.yonumen.top

[S21] C：字符类别判断
来源：http://udj.vehdjk.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xni.cucudq.cn

[S22] C：字符串转数字
来源：http://cix.aibaodan.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ftm.yvedp.cn

[S23] C：随机数
来源：http://cgq.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://jfw.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://sua.fktsv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pjx.xuetiantiany.cn

[S25] C：内存拷贝
来源：http://nbs.zhixingplan.top

memcpy(dst, src, n);
来源：http://pzv.c1oappe.top

[S26] C：内存清零
来源：http://tyx.gzhubu.top

memset(a, 0, sizeof a);
来源：http://dcv.yvedp.cn

[S27] C：定义常量
来源：http://gaz.jqgfzy.top

const double PI = 3.14159;
来源：http://nwi.shanyushiyangtech.top

[S28] C：静态变量
来源：http://ghk.feifeiyinyue.top

static int counter = 0;
来源：http://fsl.andypj.xyz

[S29] C：变参函数
来源：http://kkr.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hsi.mhx1999.top

[S30] C：头文件保护
来源：http://agy.fktsv.cn

#ifndef X_H
来源：http://nvl.jqgufenzy.top

#define X_H
来源：http://hji.fktsv.cn

#endif
来源：http://alk.hywenlv.cn

[S31] C++：Hello World
来源：http://adk.pengpengdd.cyou

#include <iostream>
来源：http://gxw.xziqi.cn

int main() { std::cout << "Hello\n"; }
来源：http://obm.fehbvm.com

[S32] C++：字符串
来源：http://seb.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://bkp.cucudq.cn

[S33] C++：vector 增删
来源：http://ocj.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rce.fktsv.cn

[S34] C++：遍历 vector
来源：http://can.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://xto.tian-w.cn

[S35] C++：map
来源：http://jvu.smart0.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ytf.uphjek.com

[S36] C++：unordered_map
来源：http://wje.aibaodan.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sow.cdnleiting.top

[S37] C++：set
来源：http://vwr.hongshengwenyu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cdq.jinyuanbaomall.cn

[S38] C++：排序
来源：http://egt.shanyushiyangtech.top

std::sort(v.begin(), v.end());
来源：http://taf.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://xyu.zycfv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qyz.ctjpmb.com

[S40] C++：查找元素
来源：http://ndz.fzhhl.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sbq.chenzaomai.com

[S41] C++：类与构造函数
来源：http://yjr.hnxiangtu.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tqr.yj20258888.top

[S42] C++：继承与虚函数
来源：http://jzm.cdnleiting.top

class B : public Base { public: void f() override {} };
来源：http://cck.shzxlz.cn

[S43] C++：智能指针
来源：http://opa.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://kxs.jqgfzy.top

[S44] C++：引用传参
来源：http://ccz.feifeiyinyue.top

void inc(int &x) { ++x; }
来源：http://kii.nanxinkj.top

[S45] C++：lambda
来源：http://pvi.chenzaomai.com

auto add = [](int a, int b) { return a + b; };
来源：http://dht.iojbl.cn

[S46] C++：函数模板
来源：http://wyx.jyoumei.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zhu.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://iqn.ppjwa.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yce.xylfe.cn

[S48] C++：逐行读文件
来源：http://ipc.jinqigfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://zer.yj202588.top

while (std::getline(in, line)) { }
来源：http://cxa.hongshengwenyu.top

[S49] C++：写文件
来源：http://lxt.sxryk.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ltr.hnxiangtu.top

[S50] C++：格式化数字
来源：http://bdp.zhiwuduotai.top


<!-- 参考信息 -->