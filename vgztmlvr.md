代发 wailian999

[Q82] 字符长度与字节长度
来源：http://ybm.chenzaomai.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zfh.zycfv.cn

[Q83] 大小写转换
来源：http://sfm.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hak.zhiwuduotai.top

[Q84] 去除首尾空格
来源：http://yyp.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://krt.shuidangran.top

[Q85] 数值取整
来源：http://cvu.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tfm.havefunace.top

[Q86] 读取 JSON 字段
来源：http://btp.wangshuangyany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bth.feifeiyinyue.top

[Q87] JSON 字段做条件
来源：http://djm.zhaomingkeji.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://llk.daria6918.cn

[Q88] 行转列（条件聚合）
来源：http://wgn.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rrp.pycfn.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dyo.tanke756.top

[Q89] 判断表是否存在
来源：http://iwj.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://iou.sxryk.cn

[Q90] 生成序号列
来源：http://yxz.xuanzx.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lpl.cqqwz.cn

================================================================================
来源：http://fmt.meibo888.top

R. Bash 专题
来源：http://grt.aibaodan.cn

================================================================================
来源：http://zxk.pengpengdd.cyou

[R01] shebang 与严格模式
来源：http://fpj.jinyuanbaomall.cn

#!/usr/bin/env bash
来源：http://tzs.dianchejie.cn

set -euo pipefail
来源：http://uxk.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://vci.cheryme.top

name="Tom"; echo "$name"
来源：http://yyv.nanxinkj.top

[R03] 只读变量
来源：http://hye.gogol.net.cn

readonly PI=3.14
来源：http://ggl.cucudq.cn

[R04] 位置参数
来源：http://jpq.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://gtc.shzxlz.cn

[R05] 参数默认值
来源：http://kut.0kj1m.cn

name="${1:-default}"
来源：http://kyc.sysykeji.top

[R06] 判断命令是否存在
来源：http://gzc.jinqigfzy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://drj.hywenlv.cn

[R07] if 判断文件
来源：http://feh.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://npy.hnqzz.top

[R08] 数值比较
来源：http://bqw.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://koh.hesvh.cn

[R09] 字符串比较
来源：http://jvq.cucudq.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mri.yfazqb.com

[R10] 正则匹配
来源：http://epr.vqdsnc.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rwg.xziqi.cn

[R11] case 多分支
来源：http://ahi.pycfn.com

case "$1" in
来源：http://oeo.nanxinkj.top

start) echo "启动" ;;
来源：http://fls.sweek.top

stop)  echo "停止" ;;
来源：http://ywc.bjfxy.top

*)     echo "未知命令" ;;
来源：http://vev.nwbrower.top

esac
来源：http://hrd.fanxiaobao.xyz

[R12] for 遍历文件
来源：http://gav.cheryme.top

for f in *.txt; do echo "$f"; done
来源：http://gne.fktsv.cn

[R13] for 计数循环
来源：http://eng.zdbjq.cn

for i in {1..10}; do echo "$i"; done
来源：http://rds.feifeiyinyue.top

[R14] C 风格 for
来源：http://iyq.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fxl.vqdsnc.cn

[R15] while 逐行读文件
来源：http://aks.bbcook.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://axm.zhiwuduotai.top

[R16] until 等待条件
来源：http://qod.xingfuxueyuan.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cxi.havefunace.top

[R17] 数组定义与取值
来源：http://jjc.svipenyu.cn

arr=(a b c); echo "${arr[0]}"
来源：http://amt.gzhubu.top

[R18] 遍历数组
来源：http://cvx.dashuyun.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jvn.cheryme.top

[R19] 数组长度
来源：http://mym.chenzaomai.com

echo "${#arr[@]}"
来源：http://bfv.yueranfly.top

[R20] 关联数组（字典）
来源：http://raz.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xiw.0kj1m.cn

[R21] 字符串长度
来源：http://nfn.uphjek.com

echo "${#s}"
来源：http://xav.fanxiaobao.xyz

[R22] 截取子串
来源：http://vte.zhijiandao.cn

echo "${s:0:5}"
来源：http://jkc.hfpthk.cn

[R23] 字符串替换
来源：http://jee.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gcv.ivvv.top

[R24] 大小写转换
来源：http://ooz.chenlongwang.top

echo "${s^^}"; echo "${s,,}"
来源：http://rxs.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://wzj.yonumen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://jzd.cqqwz.cn

[R26] 命令替换
来源：http://uqy.sjlbkw.cn

now=$(date +%F); echo "$now"
来源：http://vkn.zhoulong.xyz

[R27] 算术展开
来源：http://sat.birdmap.top

echo $((1 + 2 * 3))
来源：http://ccg.zhaomingkeji.xyz

[R28] 浮点运算
来源：http://lvm.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://unf.hongshengwenyu.top

[R29] 定义函数
来源：http://gaq.wangshuangyany.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uks.yueranfly.top

[R30] 函数返回状态码
来源：http://gcj.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://wjb.chenjidiqi.icu

[R31] 局部变量
来源：http://weq.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://hjt.jinqigufen.top

[R32] 参数个数校验
来源：http://xwc.yvedp.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://moq.52xcode.cn

[R33] 捕获错误并提示行号
来源：http://fmj.iojbl.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://czu.nanxuanxn.top

[R34] 退出时清理
来源：http://ivj.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://jbn.nanxinkj.top

[R35] 后台执行并等待
来源：http://put.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ymj.fehbvm.com

[R36] 并发执行多个任务
来源：http://pci.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://rvu.c1oappe.top

[R37] 把输出赋给变量
来源：http://qnr.wangshuangyany.cn

files=$(ls -1)
来源：http://gxt.9152youxi.cn

[R38] 管道串联
来源：http://lzc.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://mtr.hammf.cn

[R39] 重定向标准输出与错误
来源：http://cqc.zhengqikj.top

cmd > out.log 2>&1
来源：http://feg.epnwcf.com

[R40] 追加写日志
来源：http://kgj.hfpthk.cn

echo "log" >> out.log
来源：http://ozl.0kj1m.cn

[R41] 丢弃输出
来源：http://ury.chenjidiqi.icu

cmd >/dev/null 2>&1
来源：http://nrj.vehdjk.com

[R42] 输入重定向
来源：http://rng.xinyue.icu

wc -l < a.txt
来源：http://bur.hnqzz.top

[R43] 按名字查找文件
来源：http://dug.jinqigfzy.top

find . -name "*.log" -type f
来源：http://iil.bbcook.cn

[R44] 按修改时间查找
来源：http://oyu.yueranfly.top

find . -mtime -7 -type f
来源：http://myv.xuanzx.com

[R45] 批量删除
来源：http://rpb.zhiwuduotai.top

find . -name "*.tmp" -delete
来源：http://wyp.gzhubu.top

[R46] 递归替换文件内容
来源：http://upx.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hmm.9152youxi.cn

[R47] sed 单行替换
来源：http://kre.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://gde.yangfankeji.com

[R48] awk 取指定列
来源：http://awf.cqqwz.cn

awk '{print $1, $3}' a.txt
来源：http://nqr.jlsjyb.cn

[R49] awk 带条件
来源：http://zuv.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zrq.fehbvm.com

[R50] awk 求和
来源：http://zvv.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pzz.shangyingyoupin.top

[R51] 排序去重取前几
来源：http://zpl.sweek.top

sort a.txt | uniq -c | sort -rn | head
来源：http://fix.pengpengdd.cyou

[R52] 统计行数
来源：http://fqs.hnxiangtu.top

wc -l a.txt
来源：http://xev.gzhubu.top

[R53] 查看文件头与实时尾
来源：http://vej.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gsl.cheryme.top

[R54] 比较两个文件
来源：http://tuo.zhiwuduotai.top

diff a.txt b.txt
来源：http://jtn.hcnkem.com

[R55] 压缩与解压
来源：http://ahx.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fsj.mhx1999.top

[R56] 远程拷贝
来源：http://sqo.ivvv.top

scp file user@host:/path/
来源：http://mwz.feifeiyinyue.top

[R57] 远程执行命令
来源：http://ylw.haohaochexian.top

ssh user@host 'uptime'
来源：http://noy.tarul.cn

[R58] 下载文件
来源：http://nsf.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vhd.vqdsnc.cn

[R59] 发 POST JSON
来源：http://jey.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tlm.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://uok.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xaw.andypj.xyz

[R61] 磁盘占用
来源：http://itw.aibaodan.cn

df -h;  du -sh *
来源：http://utx.nanxinkj.top

[R62] 找最占空间的文件
来源：http://ouj.yuanzhike.top

du -ah . | sort -rh | head -10
来源：http://oqh.svipenyu.cn

[R63] 内存与进程
来源：http://cse.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://dhg.zhoulong.xyz

[R64] 结束进程
来源：http://bje.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://zdg.zhongyouzk.top

[R65] 查看端口占用
来源：http://hof.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://urk.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://tzk.kuanghao11.cn

crontab -e;  crontab -l
来源：http://rch.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://luk.yongpay.top

openssl rand -hex 16
来源：http://cuy.yj202588.top

[R68] 计算文件校验值
来源：http://srd.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://yaj.dashuyun.cn

[R69] 生成随机密码
来源：http://vlo.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://qaw.ybcxt.top

[R70] 时间戳与互转
来源：http://vpj.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://ezc.jianghu66.top

[R71] 日期格式化
来源：http://cab.ybcxt.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://mcq.yueranfly.top

[R72] 等待端口就绪
来源：http://fkq.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lll.nanxinkj.top

[R73] 分割大日志
来源：http://gkj.daria6918.cn

split -l 1000 big.log part_
来源：http://fnn.ctjpmb.com

[R74] 批量重命名
来源：http://chc.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vzy.cashguo.top

[R75] 导出环境变量
来源：http://kth.smart0.xyz

export PATH="$HOME/bin:$PATH"
来源：http://dyr.ehwqpu.com

[R76] 使用临时文件
来源：http://hrl.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dew.tianlin.xyz

[R77] 读取用户输入
来源：http://vxh.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://cew.vehdjk.com

[R78] 交互式菜单
来源：http://vld.yj20258.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fbi.sxryk.cn

[R79] 解析命令行选项
来源：http://ktl.hywenlv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yat.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://cdj.shanyushiyangtech.top

time ./run.sh
来源：http://irm.yanxiufei.cn

================================================================================
来源：http://xfh.xuanzx.com

S. C / C++ 专题
来源：http://ovh.dianchejie.cn

================================================================================
来源：http://tnk.jyoumei.cn

[S01] C：Hello World
来源：http://uka.birdmap.top

#include <stdio.h>
来源：http://tyu.yangfankeji.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://pfb.zhaomingkeji.xyz

[S02] C：变量与格式化输出
来源：http://tax.tanke756.top

int a = 10; printf("%d\n", a);
来源：http://kra.havefunace.top

[S03] C：读入整数
来源：http://zyj.shuidangran.top

int x; scanf("%d", &x);
来源：http://ouc.jinqigfzy.top

[S04] C：字符串复制
来源：http://vjd.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cpp.iojbl.cn

[S05] C：字符串长度
来源：http://iie.fktsv.cn

strlen(s)
来源：http://cgg.52xcode.cn

[S06] C：字符串比较
来源：http://jwe.cucudq.cn

strcmp(a, b) == 0
来源：http://lcw.yj202588.top

[S07] C：数组遍历求和
来源：http://scp.jyoumei.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wxq.havefunace.top

[S08] C：动态内存分配与释放
来源：http://dwv.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jor.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://tff.nwbrower.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://erk.hammf.cn

[S10] C：指针与解引用
来源：http://nlr.uphjek.com

int *p = &a;  *p = 5;
来源：http://qbj.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://jfj.quarkkingdee.top

FILE *f = fopen("a.txt", "r");
来源：http://xrs.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hlj.zhiwuduotai.top

fclose(f);
来源：http://qza.bjfxy.top

[S12] C：写文件
来源：http://mus.yongpay.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kll.yj20258888.top

[S13] C：宏定义
来源：http://ylx.quarkkingdee.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iko.kuanghao11.cn

[S14] C：枚举
来源：http://rwu.hongshengwenyu.top

enum Color { RED, GREEN, BLUE };
来源：http://exy.jiagoushi.top

[S15] C：类型转换
来源：http://vue.fengsongda.top

(double) a / b
来源：http://ubb.jlsjyb.cn

[S16] C：位操作置位
来源：http://gle.havefunace.top

x |= (1 << 3);
来源：http://sly.cucudq.cn

[S17] C：安全拼接字符串
来源：http://sdt.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zwn.xingfuxueyuan.xyz

[S18] C：命令行参数
来源：http://bef.sweek.top

int main(int argc, char **argv)
来源：http://xcv.vqdsnc.cn

[S19] C：快速排序
来源：http://wjj.hywenlv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jtr.cdnleiting.top

[S20] C：二分查找
来源：http://gsd.dianchejie.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oti.havefunace.top

[S21] C：字符类别判断
来源：http://aib.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mpb.hysaishi.cn

[S22] C：字符串转数字
来源：http://mia.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://caw.redwolf501.top

[S23] C：随机数
来源：http://ldb.xziqi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rai.ywan-chungtsiang.top

[S24] C：获取本地时间
来源：http://stb.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yzu.sysykeji.top

[S25] C：内存拷贝
来源：http://yem.shuidangran.top

memcpy(dst, src, n);
来源：http://evj.guannengcc.top

[S26] C：内存清零
来源：http://tlv.yj202588.top

memset(a, 0, sizeof a);
来源：http://xvy.mhx1999.top

[S27] C：定义常量
来源：http://lsw.ivvv.top

const double PI = 3.14159;
来源：http://kem.zhongyouzk.top

[S28] C：静态变量
来源：http://qtl.zhaomingkeji.xyz

static int counter = 0;
来源：http://qls.0kj1m.cn

[S29] C：变参函数
来源：http://glo.chenjidiqi.icu

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wbd.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://ebj.dashuyun.cn

#ifndef X_H
来源：http://tte.xuanzx.com

#define X_H
来源：http://kmg.shanyushiyangkeji.top

#endif
来源：http://aej.yonumen.top

[S31] C++：Hello World
来源：http://gcv.hywenlv.cn

#include <iostream>
来源：http://bed.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://qce.yongpay.top

[S32] C++：字符串
来源：http://itl.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://ulq.zdbjq.cn

[S33] C++：vector 增删
来源：http://sbk.cheryme.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://skl.sjlbkw.cn

[S34] C++：遍历 vector
来源：http://kuc.ehwqpu.com

for (auto &x : v) { std::cout << x; }
来源：http://fpo.ywan-chungtsiang.top

[S35] C++：map
来源：http://mrp.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yum.haohaochexian.top

[S36] C++：unordered_map
来源：http://kes.vehdjk.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ete.sysykeji.top

[S37] C++：set
来源：http://pbk.birdmap.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cgu.fzhhl.top

[S38] C++：排序
来源：http://yws.mhx1999.top

std::sort(v.begin(), v.end());
来源：http://qsd.guannengcc.top

[S39] C++：自定义比较器排序
来源：http://bas.sjlbkw.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cig.bjfxy.top

[S40] C++：查找元素
来源：http://qvr.aizwys.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahc.uphjek.com

[S41] C++：类与构造函数
来源：http://ezj.nwbrower.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://klm.jqgufenzy.top

[S42] C++：继承与虚函数
来源：http://fvb.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://jrk.jianghu66.top

[S43] C++：智能指针
来源：http://xhl.wangdashe.top

auto p = std::make_unique<int>(5);
来源：http://vrp.zhijiandao.cn

[S44] C++：引用传参
来源：http://gcl.vehdjk.com

void inc(int &x) { ++x; }
来源：http://jhq.fzhhl.top

[S45] C++：lambda
来源：http://ehh.yueranfly.top

auto add = [](int a, int b) { return a + b; };
来源：http://fvy.xinyue.icu

[S46] C++：函数模板
来源：http://wds.ywan-chungtsiang.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bnr.jinghuilouyu.cn

[S47] C++：结构化绑定遍历
来源：http://giv.sysykeji.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hyd.shuidangran.top

[S48] C++：逐行读文件
来源：http://skz.yangfankeji.com

std::ifstream in("a.txt");  std::string line;
来源：http://utb.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://czb.ctjpmb.com

[S49] C++：写文件
来源：http://qff.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jyz.xuanzx.com

[S50] C++：格式化数字
来源：http://hvn.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hhw.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://kio.chenlongwang.top

static_cast<double>(a) / b
来源：http://ccu.gzhubu.top

[S52] C++：const 与 noexcept
来源：http://lbx.yongpay.top


<!-- 参考信息 -->