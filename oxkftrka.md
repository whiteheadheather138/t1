代发 wailian999

[Q80] 字符串截取
来源：http://xfj.pycfn.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ihc.fzhhl.top

[Q81] 字符串替换
来源：http://gbw.xylfe.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ibj.jinqigfzy.top

[Q82] 字符长度与字节长度
来源：http://wza.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://djm.nanxuanxn.top

[Q83] 大小写转换
来源：http://deb.yj20258.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nna.0kj1m.cn

[Q84] 去除首尾空格
来源：http://qzf.c1oappe.top

SELECT TRIM(name) FROM users;
来源：http://aco.sweek.top

[Q85] 数值取整
来源：http://xww.zhongyouzk.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vav.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://uar.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cpu.pengpengdd.cyou

[Q87] JSON 字段做条件
来源：http://fpa.pengpengdd.cyou

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lay.chenzaomai.com

[Q88] 行转列（条件聚合）
来源：http://wbm.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://htl.jinqigufen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://oap.chenzaomai.com

[Q89] 判断表是否存在
来源：http://lwm.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uqh.sysykeji.top

[Q90] 生成序号列
来源：http://hoi.hammf.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kff.kuanghao11.cn

================================================================================
来源：http://zgl.316326.xyz

R. Bash 专题
来源：http://egv.zhengqikj.top

================================================================================
来源：http://hqo.chenzaomai.com

[R01] shebang 与严格模式
来源：http://ino.jyoumei.cn

#!/usr/bin/env bash
来源：http://hmz.pycfn.com

set -euo pipefail
来源：http://aeg.ivvv.top

[R02] 变量赋值与使用
来源：http://nrf.birdmap.top

name="Tom"; echo "$name"
来源：http://fic.ywan-chungtsiang.top

[R03] 只读变量
来源：http://idc.dianchejie.cn

readonly PI=3.14
来源：http://qbs.mhx1999.top

[R04] 位置参数
来源：http://olx.fehbvm.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lfg.316326.xyz

[R05] 参数默认值
来源：http://ifm.xylfe.cn

name="${1:-default}"
来源：http://ppy.ywan-chungtsiang.top

[R06] 判断命令是否存在
来源：http://exf.bbcook.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kmx.0kj1m.cn

[R07] if 判断文件
来源：http://nwe.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://onb.fanxiaobao.xyz

[R08] 数值比较
来源：http://qwx.aizwys.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vnb.zhoulong.xyz

[R09] 字符串比较
来源：http://ltg.shuidangran.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gxj.jlsjyb.cn

[R10] 正则匹配
来源：http://taa.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jil.ydjk.org.cn

[R11] case 多分支
来源：http://lvr.gzhubu.top

case "$1" in
来源：http://lfb.yfazqb.com

start) echo "启动" ;;
来源：http://iir.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://fbg.xuetiantiany.cn

*)     echo "未知命令" ;;
来源：http://djs.quarkkingdee.top

esac
来源：http://gof.uphjek.com

[R12] for 遍历文件
来源：http://nyn.ydzc1.top

for f in *.txt; do echo "$f"; done
来源：http://hau.cdnleiting.top

[R13] for 计数循环
来源：http://lsq.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://zmg.hfpthk.cn

[R14] C 风格 for
来源：http://eha.chenzaomai.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gcb.cdnleiting.top

[R15] while 逐行读文件
来源：http://wfs.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bam.dianchejie.cn

[R16] until 等待条件
来源：http://lbu.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://crj.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://bmo.jqgufenzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://kxn.ywan-chungtsiang.top

[R18] 遍历数组
来源：http://kxl.yj20258888.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ddk.jianghu66.top

[R19] 数组长度
来源：http://qyn.zhijiandao.cn

echo "${#arr[@]}"
来源：http://uwo.birdmap.top

[R20] 关联数组（字典）
来源：http://tox.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oba.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://ery.zdqjudy.top

echo "${#s}"
来源：http://eao.zhengqikj.top

[R22] 截取子串
来源：http://oqe.316326.xyz

echo "${s:0:5}"
来源：http://nuy.zdbjq.cn

[R23] 字符串替换
来源：http://vwg.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://odv.fengsongda.top

[R24] 大小写转换
来源：http://txm.gogol.net.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xku.yueranfly.top

[R25] 去后缀 / 去前缀
来源：http://wxr.hcnkem.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://vlw.yuxming.cn

[R26] 命令替换
来源：http://bfx.316326.xyz

now=$(date +%F); echo "$now"
来源：http://etd.feifeiyinyue.top

[R27] 算术展开
来源：http://hpk.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://pfk.nanxinkj.top

[R28] 浮点运算
来源：http://pwm.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://trp.xylfe.cn

[R29] 定义函数
来源：http://ycd.bjfxy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gfm.xingfuxueyuan.xyz

[R30] 函数返回状态码
来源：http://kqg.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://fru.fehbvm.com

[R31] 局部变量
来源：http://lrk.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://qfw.dianchejie.cn

[R32] 参数个数校验
来源：http://zfd.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gdq.iojbl.cn

[R33] 捕获错误并提示行号
来源：http://iku.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wxn.yonumen.top

[R34] 退出时清理
来源：http://jfk.xinyue.icu

trap 'rm -f "$tmp"' EXIT
来源：http://zar.c1oappe.top

[R35] 后台执行并等待
来源：http://kvh.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zeh.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://zqu.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fkx.wangdashe.top

[R37] 把输出赋给变量
来源：http://don.fanxiaobao.xyz

files=$(ls -1)
来源：http://boy.sysykeji.top

[R38] 管道串联
来源：http://kac.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://rlm.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://cis.hnqzz.top

cmd > out.log 2>&1
来源：http://cuf.hnxiangtu.top

[R40] 追加写日志
来源：http://vqx.jinqigufen.top

echo "log" >> out.log
来源：http://ecn.yueranfly.top

[R41] 丢弃输出
来源：http://jcd.jlsjyb.cn

cmd >/dev/null 2>&1
来源：http://xql.ydzc1.top

[R42] 输入重定向
来源：http://kau.sweek.top

wc -l < a.txt
来源：http://wie.52xcode.cn

[R43] 按名字查找文件
来源：http://ewe.hesvh.cn

find . -name "*.log" -type f
来源：http://khl.jinqigufen.top

[R44] 按修改时间查找
来源：http://zxo.shangyingyoupin.top

find . -mtime -7 -type f
来源：http://axy.zhiwuduotai.top

[R45] 批量删除
来源：http://tgf.birdmap.top

find . -name "*.tmp" -delete
来源：http://lit.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://mkh.havefunace.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ihf.uphjek.com

[R47] sed 单行替换
来源：http://mcb.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://fdf.tianlin.xyz

[R48] awk 取指定列
来源：http://atp.jinghuilouyu.cn

awk '{print $1, $3}' a.txt
来源：http://qgs.svipenyu.cn

[R49] awk 带条件
来源：http://ffb.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qka.zhijiandao.cn

[R50] awk 求和
来源：http://pmo.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://jec.sufxvd.cn

[R51] 排序去重取前几
来源：http://sar.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vhh.yonumen.top

[R52] 统计行数
来源：http://evn.tianlin.xyz

wc -l a.txt
来源：http://jpy.cashguo.top

[R53] 查看文件头与实时尾
来源：http://rur.zhijiandao.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hlv.chenlongwang.top

[R54] 比较两个文件
来源：http://nhk.ybcxt.top

diff a.txt b.txt
来源：http://isz.yuanzhike.top

[R55] 压缩与解压
来源：http://okc.sufxvd.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uqw.ppjwa.cn

[R56] 远程拷贝
来源：http://age.zhijiandao.cn

scp file user@host:/path/
来源：http://zfn.ivvv.top

[R57] 远程执行命令
来源：http://iag.ehwqpu.com

ssh user@host 'uptime'
来源：http://ogf.yueranfly.top

[R58] 下载文件
来源：http://cud.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kov.yongpay.top

[R59] 发 POST JSON
来源：http://ucn.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vcm.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://pli.dashuyun.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nis.mhx1999.top

[R61] 磁盘占用
来源：http://ilh.hfpthk.cn

df -h;  du -sh *
来源：http://dfc.hcnkem.com

[R62] 找最占空间的文件
来源：http://pxi.nanxuanxn.top

du -ah . | sort -rh | head -10
来源：http://hcg.andypj.xyz

[R63] 内存与进程
来源：http://iwm.9152youxi.cn

free -h;  ps aux | grep nginx
来源：http://tsn.jyoumei.cn

[R64] 结束进程
来源：http://nkt.ydjk.org.cn

kill -9 $(pgrep -f app.py)
来源：http://ymv.jianghu66.top

[R65] 查看端口占用
来源：http://hye.yuxming.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jnn.chenzaomai.com

[R66] 定时任务
来源：http://qnn.zhongyouzk.top

crontab -e;  crontab -l
来源：http://bpu.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://ont.yvedp.cn

openssl rand -hex 16
来源：http://phw.yj202588.top

[R68] 计算文件校验值
来源：http://kig.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tzc.ivvv.top

[R69] 生成随机密码
来源：http://shf.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://clc.sxryk.cn

[R70] 时间戳与互转
来源：http://ynf.svipenyu.cn

date +%s;  date -d @1700000000
来源：http://lnt.haohaochexian.top

[R71] 日期格式化
来源：http://feq.xingfuxueyuan.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://vam.hfpthk.cn

[R72] 等待端口就绪
来源：http://lbj.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://hcb.fengsongda.top

[R73] 分割大日志
来源：http://kiq.52xcode.cn

split -l 1000 big.log part_
来源：http://cnc.vehdjk.com

[R74] 批量重命名
来源：http://xlt.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://unf.jqgfzy.top

[R75] 导出环境变量
来源：http://vew.sjlbkw.cn

export PATH="$HOME/bin:$PATH"
来源：http://udg.cheryme.top

[R76] 使用临时文件
来源：http://yjh.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://eyc.kuanghao11.cn

[R77] 读取用户输入
来源：http://vdb.daxiang520.top

read -rp "请输入: " ans
来源：http://hct.gaohongyu789.top

[R78] 交互式菜单
来源：http://rnr.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://nza.nwbrower.top

[R79] 解析命令行选项
来源：http://pci.chenjidiqi.icu

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://drq.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://omc.jiagoushi.top

time ./run.sh
来源：http://ngm.hesvh.cn

================================================================================
来源：http://rma.hesvh.cn

S. C / C++ 专题
来源：http://fmj.nanxinkj.top

================================================================================
来源：http://frc.fzhhl.top

[S01] C：Hello World
来源：http://kus.52xcode.cn

#include <stdio.h>
来源：http://bjl.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rva.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://fal.jlsjyb.cn

int a = 10; printf("%d\n", a);
来源：http://yrl.yanxiufei.cn

[S03] C：读入整数
来源：http://xyv.iojbl.cn

int x; scanf("%d", &x);
来源：http://ifu.havefunace.top

[S04] C：字符串复制
来源：http://wqg.bjfxy.top

char dst[32]; strcpy(dst, "hi");
来源：http://gjp.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://zya.wangshuangyany.cn

strlen(s)
来源：http://oum.nanxuanxn.top

[S06] C：字符串比较
来源：http://yfi.fehbvm.com

strcmp(a, b) == 0
来源：http://ylw.hnqzz.top

[S07] C：数组遍历求和
来源：http://rtx.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zah.yj202588.top

[S08] C：动态内存分配与释放
来源：http://phm.cdnleiting.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://udr.havefunace.top

[S09] C：结构体定义与初始化
来源：http://ils.zhengqikj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kzt.zhongyouzk.top

[S10] C：指针与解引用
来源：http://ulr.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://hcf.aizwys.cn

[S11] C：逐行读文件
来源：http://bil.hnqzz.top

FILE *f = fopen("a.txt", "r");
来源：http://kcj.jinqigfzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nms.ctjpmb.com

fclose(f);
来源：http://pbb.bjfxy.top

[S12] C：写文件
来源：http://auh.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hql.hnxiangtu.top

[S13] C：宏定义
来源：http://nhx.cashguo.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mtz.ivvv.top

[S14] C：枚举
来源：http://puj.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://orw.hammf.cn

[S15] C：类型转换
来源：http://pte.jiagoushi.top

(double) a / b
来源：http://ouh.tarul.cn

[S16] C：位操作置位
来源：http://vao.meibo888.top

x |= (1 << 3);
来源：http://xdl.jqgufenzy.top

[S17] C：安全拼接字符串
来源：http://dyv.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ctm.jinqigufen.top

[S18] C：命令行参数
来源：http://zef.hywenlv.cn

int main(int argc, char **argv)
来源：http://qfg.zhiwuduotai.top

[S19] C：快速排序
来源：http://kbw.zhixingplan.top

qsort(a, n, sizeof(int), cmp);
来源：http://ljf.xuetiantiany.cn

[S20] C：二分查找
来源：http://qtl.bjfxy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ixx.cucudq.cn

[S21] C：字符类别判断
来源：http://ypm.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://abe.ybcxt.top

[S22] C：字符串转数字
来源：http://bjd.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qgk.zdqjudy.top

[S23] C：随机数
来源：http://wjc.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://aen.zhijiandao.cn

[S24] C：获取本地时间
来源：http://gnn.ppjwa.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wuw.jianghu66.top

[S25] C：内存拷贝
来源：http://hhs.daxiang520.top

memcpy(dst, src, n);
来源：http://oma.zhixingplan.top

[S26] C：内存清零
来源：http://sdh.fanxiaobao.xyz

memset(a, 0, sizeof a);
来源：http://jrq.xziqi.cn

[S27] C：定义常量
来源：http://mrg.yonumen.top

const double PI = 3.14159;
来源：http://xjd.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://oex.sjlbkw.cn

static int counter = 0;
来源：http://wqu.shuidangran.top

[S29] C：变参函数
来源：http://dcu.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mim.bjfxy.top

[S30] C：头文件保护
来源：http://dra.52xcode.cn

#ifndef X_H
来源：http://ugf.cheryme.top

#define X_H
来源：http://tpk.yfazqb.com

#endif
来源：http://jlg.nanxuanxn.top

[S31] C++：Hello World
来源：http://mtw.yueranfly.top

#include <iostream>
来源：http://wki.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://qno.bjfxy.top

[S32] C++：字符串
来源：http://pko.hongshengwenyu.top

std::string s = "hi";  s += "!";
来源：http://igh.smart0.xyz

[S33] C++：vector 增删
来源：http://fyk.bbcook.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uum.sweek.top

[S34] C++：遍历 vector
来源：http://cpw.andypj.xyz

for (auto &x : v) { std::cout << x; }
来源：http://hrw.aibaodan.cn

[S35] C++：map
来源：http://iso.mhx1999.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://anr.wangdashe.top

[S36] C++：unordered_map
来源：http://vdr.dashuyun.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zfg.chenzaomai.com

[S37] C++：set
来源：http://obx.ywan-chungtsiang.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://udl.xylfe.cn

[S38] C++：排序
来源：http://mxd.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://qmn.316326.xyz

[S39] C++：自定义比较器排序
来源：http://fos.tarul.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hrn.svipenyu.cn

[S40] C++：查找元素
来源：http://ltp.yfazqb.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://txk.xziqi.cn

[S41] C++：类与构造函数
来源：http://qdd.hammf.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yyu.smart0.xyz

[S42] C++：继承与虚函数
来源：http://naq.sufxvd.cn

class B : public Base { public: void f() override {} };
来源：http://nsd.yuanzhike.top

[S43] C++：智能指针
来源：http://wxj.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://xam.jianghu66.top

[S44] C++：引用传参
来源：http://xes.shanyushiyangtech.top

void inc(int &x) { ++x; }
来源：http://ety.dashuyun.cn

[S45] C++：lambda
来源：http://srf.feifeiyinyue.top

auto add = [](int a, int b) { return a + b; };
来源：http://emy.kuanghao11.cn

[S46] C++：函数模板
来源：http://nim.hnxiangtu.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fgy.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://jol.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfv.sweek.top

[S48] C++：逐行读文件
来源：http://jst.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://xaw.yangfankeji.com

while (std::getline(in, line)) { }
来源：http://fwi.havefunace.top

[S49] C++：写文件
来源：http://clz.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eqn.hysaishi.cn

[S50] C++：格式化数字
来源：http://vju.316326.xyz


<!-- 参考信息 -->