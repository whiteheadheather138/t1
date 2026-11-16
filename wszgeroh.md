代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://hpt.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://nsw.xingfuxueyuan.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qaz.zhoulong.xyz

[Q89] 判断表是否存在
来源：http://dvl.jinqigufen.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ixn.chenzaomai.com

[Q90] 生成序号列
来源：http://alf.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bjb.yj202588.top

================================================================================
来源：http://dzf.daria6918.cn

R. Bash 专题
来源：http://lah.daxiang520.top

================================================================================
来源：http://sgt.yj20258.top

[R01] shebang 与严格模式
来源：http://imp.zhongyouzk.top

#!/usr/bin/env bash
来源：http://qfb.aibaodan.cn

set -euo pipefail
来源：http://rvw.andypj.xyz

[R02] 变量赋值与使用
来源：http://shx.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://ggs.jianghu66.top

[R03] 只读变量
来源：http://nqm.hfpthk.cn

readonly PI=3.14
来源：http://yzo.uphjek.com

[R04] 位置参数
来源：http://bqv.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://aci.cashguo.top

[R05] 参数默认值
来源：http://myl.uphjek.com

name="${1:-default}"
来源：http://fwe.chenlongwang.top

[R06] 判断命令是否存在
来源：http://srz.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dvv.redwolf501.top

[R07] if 判断文件
来源：http://kea.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wnb.pengpengdd.cyou

[R08] 数值比较
来源：http://igd.tian-w.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dzk.aibaodan.cn

[R09] 字符串比较
来源：http://pqu.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ywc.guowangkeji.top

[R10] 正则匹配
来源：http://hux.fzhhl.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iej.ybcxt.top

[R11] case 多分支
来源：http://nmm.yonumen.top

case "$1" in
来源：http://abb.shuidangran.top

start) echo "启动" ;;
来源：http://mlp.snrcjt.cn

stop)  echo "停止" ;;
来源：http://siz.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://mae.tarul.cn

esac
来源：http://qcg.vqdsnc.cn

[R12] for 遍历文件
来源：http://ykb.yj20258.top

for f in *.txt; do echo "$f"; done
来源：http://geo.zhongyouzk.top

[R13] for 计数循环
来源：http://rot.daria6918.cn

for i in {1..10}; do echo "$i"; done
来源：http://lmz.xylfe.cn

[R14] C 风格 for
来源：http://jqj.gzhubu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ykz.chenzaomai.com

[R15] while 逐行读文件
来源：http://phx.snrcjt.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ype.redwolf501.top

[R16] until 等待条件
来源：http://vcu.zdbjq.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xvl.zdqjudy.top

[R17] 数组定义与取值
来源：http://rpw.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://enm.shanyushiyangtech.top

[R18] 遍历数组
来源：http://ogo.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hlg.feifeiyinyue.top

[R19] 数组长度
来源：http://kyf.feifeiyinyue.top

echo "${#arr[@]}"
来源：http://jyp.tarul.cn

[R20] 关联数组（字典）
来源：http://kgc.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mjf.52xcode.cn

[R21] 字符串长度
来源：http://naw.zhijiandao.cn

echo "${#s}"
来源：http://cvf.fengsongda.top

[R22] 截取子串
来源：http://mmt.jiagoushi.top

echo "${s:0:5}"
来源：http://cbs.ybcxt.top

[R23] 字符串替换
来源：http://zop.meibo888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aei.daria6918.cn

[R24] 大小写转换
来源：http://kad.ivvv.top

echo "${s^^}"; echo "${s,,}"
来源：http://iit.0kj1m.cn

[R25] 去后缀 / 去前缀
来源：http://kyx.epnwcf.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://qla.yj20258.top

[R26] 命令替换
来源：http://crp.fktsv.cn

now=$(date +%F); echo "$now"
来源：http://scv.tanke756.top

[R27] 算术展开
来源：http://juo.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://hmd.kuanghao11.cn

[R28] 浮点运算
来源：http://sxq.feifeiyinyue.top

echo "scale=2; 10/3" | bc
来源：http://ijp.yuanzhike.top

[R29] 定义函数
来源：http://krf.xinyue.icu

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gvz.sjlbkw.cn

[R30] 函数返回状态码
来源：http://pti.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://uqr.jinqigfzy.top

[R31] 局部变量
来源：http://ihu.hongshengwenyu.top

f() { local x=1; echo "$x"; }
来源：http://mhp.bjfxy.top

[R32] 参数个数校验
来源：http://pry.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vmv.316326.xyz

[R33] 捕获错误并提示行号
来源：http://fnw.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ige.pengpengdd.cyou

[R34] 退出时清理
来源：http://xto.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://sir.haohaochexian.top

[R35] 后台执行并等待
来源：http://ttx.gogol.net.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qvm.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://azb.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://odd.pycfn.com

[R37] 把输出赋给变量
来源：http://mlw.ivvv.top

files=$(ls -1)
来源：http://jaz.ppjwa.cn

[R38] 管道串联
来源：http://yge.0kj1m.cn

cat a.txt | grep -i error | wc -l
来源：http://svl.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://ica.yfazqb.com

cmd > out.log 2>&1
来源：http://smj.sxryk.cn

[R40] 追加写日志
来源：http://xqg.shzxlz.cn

echo "log" >> out.log
来源：http://ejq.9152youxi.cn

[R41] 丢弃输出
来源：http://cea.nanxinkj.top

cmd >/dev/null 2>&1
来源：http://exm.chenjidiqi.icu

[R42] 输入重定向
来源：http://mxa.xylfe.cn

wc -l < a.txt
来源：http://rqn.gotoacloud.top

[R43] 按名字查找文件
来源：http://eda.jyoumei.cn

find . -name "*.log" -type f
来源：http://avq.zdbjq.cn

[R44] 按修改时间查找
来源：http://fbu.sufxvd.cn

find . -mtime -7 -type f
来源：http://vmy.hfpthk.cn

[R45] 批量删除
来源：http://hdu.jinyuanbaomall.cn

find . -name "*.tmp" -delete
来源：http://fwx.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://saf.wangdashe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qot.yuxming.cn

[R47] sed 单行替换
来源：http://sgz.chenzaomai.com

sed -i 's/foo/bar/g' a.txt
来源：http://vdg.jyoumei.cn

[R48] awk 取指定列
来源：http://yze.yj202588.top

awk '{print $1, $3}' a.txt
来源：http://ykj.nanxinkj.top

[R49] awk 带条件
来源：http://wxu.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://har.xziqi.cn

[R50] awk 求和
来源：http://uwa.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xdm.ywan-chungtsiang.top

[R51] 排序去重取前几
来源：http://oxr.0kj1m.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ixr.cucudq.cn

[R52] 统计行数
来源：http://pbg.yongpay.top

wc -l a.txt
来源：http://zye.xziqi.cn

[R53] 查看文件头与实时尾
来源：http://zig.chenlongwang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xkk.birdmap.top

[R54] 比较两个文件
来源：http://ent.jinqigufen.top

diff a.txt b.txt
来源：http://ude.cucudq.cn

[R55] 压缩与解压
来源：http://ftm.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bqy.zhongyouzk.top

[R56] 远程拷贝
来源：http://vwo.pycfn.com

scp file user@host:/path/
来源：http://pia.yongpay.top

[R57] 远程执行命令
来源：http://otj.vehdjk.com

ssh user@host 'uptime'
来源：http://lwz.shzxlz.cn

[R58] 下载文件
来源：http://fgo.316326.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rsi.hysaishi.cn

[R59] 发 POST JSON
来源：http://avh.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ndk.yuxming.cn

[R60] 只看 HTTP 状态码
来源：http://jlm.yuanzhike.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qjn.0kj1m.cn

[R61] 磁盘占用
来源：http://ivp.redwolf501.top

df -h;  du -sh *
来源：http://fay.zdbjq.cn

[R62] 找最占空间的文件
来源：http://rgq.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://vak.svipenyu.cn

[R63] 内存与进程
来源：http://fyd.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://uiw.zhaomingkeji.xyz

[R64] 结束进程
来源：http://son.zdqjudy.top

kill -9 $(pgrep -f app.py)
来源：http://osj.hnqzz.top

[R65] 查看端口占用
来源：http://kxx.cucudq.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bxj.cucudq.cn

[R66] 定时任务
来源：http://ain.bjfxy.top

crontab -e;  crontab -l
来源：http://vvf.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://ahm.sufxvd.cn

openssl rand -hex 16
来源：http://yar.bbcook.cn

[R68] 计算文件校验值
来源：http://tdi.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://uzk.epnwcf.com

[R69] 生成随机密码
来源：http://amp.tianlin.xyz

head -c 16 /dev/urandom | base64
来源：http://kgd.mhx1999.top

[R70] 时间戳与互转
来源：http://rtm.birdmap.top

date +%s;  date -d @1700000000
来源：http://kvn.dashuyun.cn

[R71] 日期格式化
来源：http://enf.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lgx.cucudq.cn

[R72] 等待端口就绪
来源：http://joq.aizwys.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wqn.zhijiandao.cn

[R73] 分割大日志
来源：http://auw.bjfxy.top

split -l 1000 big.log part_
来源：http://rju.ppjwa.cn

[R74] 批量重命名
来源：http://byd.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://efz.wangshuangyany.cn

[R75] 导出环境变量
来源：http://ynl.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://vbv.aizwys.cn

[R76] 使用临时文件
来源：http://pca.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kke.jqgfzy.top

[R77] 读取用户输入
来源：http://zio.yangfankeji.com

read -rp "请输入: " ans
来源：http://aap.fzhhl.top

[R78] 交互式菜单
来源：http://iou.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qhk.yuxming.cn

[R79] 解析命令行选项
来源：http://kcr.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ufi.cheryme.top

[R80] 查看脚本执行耗时
来源：http://aco.ywan-chungtsiang.top

time ./run.sh
来源：http://vjk.tarul.cn

================================================================================
来源：http://neh.tanke756.top

S. C / C++ 专题
来源：http://azg.dashuyun.cn

================================================================================
来源：http://sik.ehwqpu.com

[S01] C：Hello World
来源：http://noi.snrcjt.cn

#include <stdio.h>
来源：http://ygu.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://pkd.pycfn.com

[S02] C：变量与格式化输出
来源：http://mtz.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://aqq.zhiwuduotai.top

[S03] C：读入整数
来源：http://uns.andypj.xyz

int x; scanf("%d", &x);
来源：http://ist.ybcxt.top

[S04] C：字符串复制
来源：http://trv.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://rwu.iojbl.cn

[S05] C：字符串长度
来源：http://bmk.hcnkem.com

strlen(s)
来源：http://qyw.hcnkem.com

[S06] C：字符串比较
来源：http://hoo.meibo888.top

strcmp(a, b) == 0
来源：http://zca.ppjwa.cn

[S07] C：数组遍历求和
来源：http://quk.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rbl.mhx1999.top

[S08] C：动态内存分配与释放
来源：http://omk.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ylb.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://keb.ivvv.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nxp.zhijiandao.cn

[S10] C：指针与解引用
来源：http://suk.yueranfly.top

int *p = &a;  *p = 5;
来源：http://hrm.shzxlz.cn

[S11] C：逐行读文件
来源：http://zcr.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://lxw.uphjek.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://vxq.yj20258.top

fclose(f);
来源：http://yhk.jqgufenzy.top

[S12] C：写文件
来源：http://dbm.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ehe.quarkkingdee.top

[S13] C：宏定义
来源：http://gpu.9152youxi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sll.bbcook.cn

[S14] C：枚举
来源：http://cxn.gzhubu.top

enum Color { RED, GREEN, BLUE };
来源：http://vwr.bbcook.cn

[S15] C：类型转换
来源：http://ejh.yj202588.top

(double) a / b
来源：http://dtl.sjlbkw.cn

[S16] C：位操作置位
来源：http://ypi.chenlongwang.top

x |= (1 << 3);
来源：http://fxh.fktsv.cn

[S17] C：安全拼接字符串
来源：http://yuv.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dnl.zhongyouzk.top

[S18] C：命令行参数
来源：http://ujj.yonumen.top

int main(int argc, char **argv)
来源：http://qdu.shangyingyoupin.top

[S19] C：快速排序
来源：http://sew.hfpthk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xao.zhengqikj.top

[S20] C：二分查找
来源：http://gnp.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tvm.hfpthk.cn

[S21] C：字符类别判断
来源：http://oyc.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qnu.yj202588.top

[S22] C：字符串转数字
来源：http://lry.svipenyu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://byf.zhongyouzk.top

[S23] C：随机数
来源：http://sau.hongshengwenyu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wnd.9152youxi.cn

[S24] C：获取本地时间
来源：http://ycw.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://red.yj202588.top

[S25] C：内存拷贝
来源：http://jqn.ehwqpu.com

memcpy(dst, src, n);
来源：http://lgg.hnqzz.top

[S26] C：内存清零
来源：http://qqv.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://mnv.redwolf501.top

[S27] C：定义常量
来源：http://jal.hywenlv.cn

const double PI = 3.14159;
来源：http://uof.bjfxy.top

[S28] C：静态变量
来源：http://fol.c1oappe.top

static int counter = 0;
来源：http://cci.52xcode.cn

[S29] C：变参函数
来源：http://zff.zhixingplan.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hms.316326.xyz

[S30] C：头文件保护
来源：http://xic.hongshengwenyu.top

#ifndef X_H
来源：http://egr.guannengcc.top

#define X_H
来源：http://wnz.hcnkem.com

#endif
来源：http://cqu.guowangkeji.top

[S31] C++：Hello World
来源：http://qzu.sufxvd.cn

#include <iostream>
来源：http://qru.dashuyun.cn

int main() { std::cout << "Hello\n"; }
来源：http://psj.zhongyouzk.top

[S32] C++：字符串
来源：http://mkt.svipenyu.cn

std::string s = "hi";  s += "!";
来源：http://tim.52xcode.cn

[S33] C++：vector 增删
来源：http://aev.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ykl.0kj1m.cn

[S34] C++：遍历 vector
来源：http://quz.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://ifm.hongshengwenyu.top

[S35] C++：map
来源：http://scr.vqdsnc.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uzy.cqqwz.cn

[S36] C++：unordered_map
来源：http://lat.vqdsnc.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://acs.zycfv.cn

[S37] C++：set
来源：http://akm.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mtx.cqqwz.cn

[S38] C++：排序
来源：http://vco.jiagoushi.top

std::sort(v.begin(), v.end());
来源：http://gmt.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://rdi.xuanzx.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qcx.chenjidiqi.icu

[S40] C++：查找元素
来源：http://osb.fanxiaobao.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hdf.hesvh.cn

[S41] C++：类与构造函数
来源：http://cux.ybcxt.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fqg.sysykeji.top

[S42] C++：继承与虚函数
来源：http://pxv.haohaochexian.top

class B : public Base { public: void f() override {} };
来源：http://tnp.chenzaomai.com

[S43] C++：智能指针
来源：http://mpm.zdbjq.cn

auto p = std::make_unique<int>(5);
来源：http://tri.zhijiandao.cn

[S44] C++：引用传参
来源：http://txr.redwolf501.top

void inc(int &x) { ++x; }
来源：http://ltf.yonumen.top

[S45] C++：lambda
来源：http://xlf.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://jjq.andypj.xyz

[S46] C++：函数模板
来源：http://jzj.yj20258888.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://teb.sweek.top

[S47] C++：结构化绑定遍历
来源：http://qis.havefunace.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tgw.xylfe.cn

[S48] C++：逐行读文件
来源：http://auz.haohaochexian.top

std::ifstream in("a.txt");  std::string line;
来源：http://vty.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://qlj.shangyingyoupin.top

[S49] C++：写文件
来源：http://yav.zdbjq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zxu.pengpengdd.cyou

[S50] C++：格式化数字
来源：http://hdh.yangfankeji.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dlu.sxryk.cn

[S51] C++：显式类型转换
来源：http://ong.hfpthk.cn

static_cast<double>(a) / b
来源：http://tzo.ehwqpu.com

[S52] C++：const 与 noexcept
来源：http://dvz.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://pzj.jqgfzy.top

[S53] C++：移动语义
来源：http://vxq.xuetiantiany.cn

std::vector<int> w = std::move(v);
来源：http://ltm.gzhubu.top

[S54] C++：异常处理
来源：http://bwv.gaohongyu789.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://son.bbcook.cn

[S55] C++：结构化绑定
来源：http://bep.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qkw.aibaodan.cn

[S56] C++：optional
来源：http://yoy.meibo888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ljz.jqgufenzy.top

[S57] C++：编译期常量
来源：http://hpw.yvedp.cn

constexpr int N = 10;
来源：http://nhn.ydjk.org.cn

[S58] C++：命名空间
来源：http://wgo.9152youxi.cn


<!-- 参考信息 -->