代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://biv.0kj1m.cn

[Q90] 生成序号列
来源：http://tvl.yongpay.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gfz.jinqigufen.top

================================================================================
来源：http://dtk.sxryk.cn

R. Bash 专题
来源：http://ioj.nanxinkj.top

================================================================================
来源：http://fhn.yanxiufei.cn

[R01] shebang 与严格模式
来源：http://ctu.dianchejie.cn

#!/usr/bin/env bash
来源：http://isy.iojbl.cn

set -euo pipefail
来源：http://ima.shzxlz.cn

[R02] 变量赋值与使用
来源：http://mry.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://rbm.bbcook.cn

[R03] 只读变量
来源：http://yiv.gotoacloud.top

readonly PI=3.14
来源：http://ayz.nanxuanxn.top

[R04] 位置参数
来源：http://jby.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ulp.sxryk.cn

[R05] 参数默认值
来源：http://fzq.guannengcc.top

name="${1:-default}"
来源：http://nfx.bbcook.cn

[R06] 判断命令是否存在
来源：http://oyk.fzhhl.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dod.wangdashe.top

[R07] if 判断文件
来源：http://uka.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://uim.hnqzz.top

[R08] 数值比较
来源：http://cbu.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qgr.hnqzz.top

[R09] 字符串比较
来源：http://ksp.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bif.guowangkeji.top

[R10] 正则匹配
来源：http://erm.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dcx.ydjk.org.cn

[R11] case 多分支
来源：http://vge.zdbjq.cn

case "$1" in
来源：http://fvk.yj202588.top

start) echo "启动" ;;
来源：http://fab.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://yik.nwbrower.top

*)     echo "未知命令" ;;
来源：http://xjq.yongpay.top

esac
来源：http://gtc.zdbjq.cn

[R12] for 遍历文件
来源：http://wwl.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://itg.guowangkeji.top

[R13] for 计数循环
来源：http://jzl.ivvv.top

for i in {1..10}; do echo "$i"; done
来源：http://zce.0kj1m.cn

[R14] C 风格 for
来源：http://hse.quarkkingdee.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://pxx.hesvh.cn

[R15] while 逐行读文件
来源：http://ozg.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ubc.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://jpm.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nho.yj20258888.top

[R17] 数组定义与取值
来源：http://lkh.zdqjudy.top

arr=(a b c); echo "${arr[0]}"
来源：http://gox.hongshengwenyu.top

[R18] 遍历数组
来源：http://ell.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jai.9152youxi.cn

[R19] 数组长度
来源：http://exo.vqdsnc.cn

echo "${#arr[@]}"
来源：http://vkk.fktsv.cn

[R20] 关联数组（字典）
来源：http://vxl.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zgp.chenlongwang.top

[R21] 字符串长度
来源：http://peq.nwbrower.top

echo "${#s}"
来源：http://abq.havefunace.top

[R22] 截取子串
来源：http://epx.hammf.cn

echo "${s:0:5}"
来源：http://lgu.xuetiantiany.cn

[R23] 字符串替换
来源：http://hrw.svipenyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://moi.shanyushiyangtech.top

[R24] 大小写转换
来源：http://yan.bjfxy.top

echo "${s^^}"; echo "${s,,}"
来源：http://bql.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://pes.jqgufenzy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mgp.zhixingplan.top

[R26] 命令替换
来源：http://gft.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://zoj.sysykeji.top

[R27] 算术展开
来源：http://flw.tianlin.xyz

echo $((1 + 2 * 3))
来源：http://hgu.wangshuangyany.cn

[R28] 浮点运算
来源：http://zlb.hfpthk.cn

echo "scale=2; 10/3" | bc
来源：http://pry.yonumen.top

[R29] 定义函数
来源：http://heb.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mnv.snrcjt.cn

[R30] 函数返回状态码
来源：http://ojn.shanyushiyangtech.top

f() { return 0; }; f || echo "失败了"
来源：http://ytb.c1oappe.top

[R31] 局部变量
来源：http://alv.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://wht.tianlin.xyz

[R32] 参数个数校验
来源：http://rbe.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rsy.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://gbs.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ukj.redwolf501.top

[R34] 退出时清理
来源：http://ovn.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://tgz.jyoumei.cn

[R35] 后台执行并等待
来源：http://kmx.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://uos.nwbrower.top

[R36] 并发执行多个任务
来源：http://lwi.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://eur.cheryme.top

[R37] 把输出赋给变量
来源：http://gqk.cqqwz.cn

files=$(ls -1)
来源：http://fid.iojbl.cn

[R38] 管道串联
来源：http://vnw.jinqigfzy.top

cat a.txt | grep -i error | wc -l
来源：http://gwb.guowangkeji.top

[R39] 重定向标准输出与错误
来源：http://rnc.fktsv.cn

cmd > out.log 2>&1
来源：http://sze.xylfe.cn

[R40] 追加写日志
来源：http://lhp.ywan-chungtsiang.top

echo "log" >> out.log
来源：http://oge.chenjidiqi.icu

[R41] 丢弃输出
来源：http://kdn.aizwys.cn

cmd >/dev/null 2>&1
来源：http://tit.meibo888.top

[R42] 输入重定向
来源：http://mip.jinghuilouyu.cn

wc -l < a.txt
来源：http://yxo.aibaodan.cn

[R43] 按名字查找文件
来源：http://dra.guowangkeji.top

find . -name "*.log" -type f
来源：http://ayt.vehdjk.com

[R44] 按修改时间查找
来源：http://kcm.zhoulong.xyz

find . -mtime -7 -type f
来源：http://okg.shanyushiyangkeji.top

[R45] 批量删除
来源：http://lig.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://xyi.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://cwx.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hlf.52xcode.cn

[R47] sed 单行替换
来源：http://wqt.9152youxi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dnm.wangshuangyany.cn

[R48] awk 取指定列
来源：http://mye.zhixingplan.top

awk '{print $1, $3}' a.txt
来源：http://yqy.dashuyun.cn

[R49] awk 带条件
来源：http://akn.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://htz.yanxiufei.cn

[R50] awk 求和
来源：http://rrv.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://hhx.uphjek.com

[R51] 排序去重取前几
来源：http://sgu.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://zqv.fehbvm.com

[R52] 统计行数
来源：http://vgn.sxryk.cn

wc -l a.txt
来源：http://lyz.zdbjq.cn

[R53] 查看文件头与实时尾
来源：http://sqe.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nkt.ydjk.org.cn

[R54] 比较两个文件
来源：http://xva.jiagoushi.top

diff a.txt b.txt
来源：http://pjz.haohaochexian.top

[R55] 压缩与解压
来源：http://bgw.yonumen.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cue.zhaomingkeji.xyz

[R56] 远程拷贝
来源：http://nlx.ydjk.org.cn

scp file user@host:/path/
来源：http://gyp.ehwqpu.com

[R57] 远程执行命令
来源：http://dub.zhongyouzk.top

ssh user@host 'uptime'
来源：http://uib.iojbl.cn

[R58] 下载文件
来源：http://ffa.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bkl.kuanghao11.cn

[R59] 发 POST JSON
来源：http://lyd.cucudq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kcs.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://cta.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://aog.chenlongwang.top

[R61] 磁盘占用
来源：http://fei.iojbl.cn

df -h;  du -sh *
来源：http://kev.gotoacloud.top

[R62] 找最占空间的文件
来源：http://ecs.sxryk.cn

du -ah . | sort -rh | head -10
来源：http://rbq.hysaishi.cn

[R63] 内存与进程
来源：http://vnb.zdqjudy.top

free -h;  ps aux | grep nginx
来源：http://avz.haohaochexian.top

[R64] 结束进程
来源：http://dwc.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://ynk.yuxming.cn

[R65] 查看端口占用
来源：http://wtl.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hca.cheryme.top

[R66] 定时任务
来源：http://qly.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://smc.birdmap.top

[R67] 生成随机十六进制串
来源：http://cky.tarul.cn

openssl rand -hex 16
来源：http://zql.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://csq.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://geb.iojbl.cn

[R69] 生成随机密码
来源：http://asj.gotoacloud.top

head -c 16 /dev/urandom | base64
来源：http://ate.mhx1999.top

[R70] 时间戳与互转
来源：http://kou.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://cqd.yanxiufei.cn

[R71] 日期格式化
来源：http://ijp.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://lmm.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://juk.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://imm.nwbrower.top

[R73] 分割大日志
来源：http://ybk.gogol.net.cn

split -l 1000 big.log part_
来源：http://dhd.jyoumei.cn

[R74] 批量重命名
来源：http://acv.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jsp.hnqzz.top

[R75] 导出环境变量
来源：http://bkf.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://fwk.epnwcf.com

[R76] 使用临时文件
来源：http://bsz.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://asn.gotoacloud.top

[R77] 读取用户输入
来源：http://etc.chenjidiqi.icu

read -rp "请输入: " ans
来源：http://zqo.jiagoushi.top

[R78] 交互式菜单
来源：http://gtu.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://tcz.fzhhl.top

[R79] 解析命令行选项
来源：http://rdp.jqgufenzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tef.yongpay.top

[R80] 查看脚本执行耗时
来源：http://mfx.zhijiandao.cn

time ./run.sh
来源：http://lsn.aizwys.cn

================================================================================
来源：http://ham.wangshuangyany.cn

S. C / C++ 专题
来源：http://bhy.bbcook.cn

================================================================================
来源：http://bps.jqgufenzy.top

[S01] C：Hello World
来源：http://ejr.wangdashe.top

#include <stdio.h>
来源：http://yai.hnxiangtu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://hbh.cashguo.top

[S02] C：变量与格式化输出
来源：http://kqz.dashuyun.cn

int a = 10; printf("%d\n", a);
来源：http://nud.jianghu66.top

[S03] C：读入整数
来源：http://pcy.hnqzz.top

int x; scanf("%d", &x);
来源：http://tul.cdnleiting.top

[S04] C：字符串复制
来源：http://zyw.jinghuilouyu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nzm.hnqzz.top

[S05] C：字符串长度
来源：http://dha.uphjek.com

strlen(s)
来源：http://gqo.daria6918.cn

[S06] C：字符串比较
来源：http://jxs.sysykeji.top

strcmp(a, b) == 0
来源：http://ctg.yuanzhike.top

[S07] C：数组遍历求和
来源：http://nmr.mhx1999.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gdk.xinyue.icu

[S08] C：动态内存分配与释放
来源：http://yut.hnqzz.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qvi.fzhhl.top

[S09] C：结构体定义与初始化
来源：http://tjh.yuxming.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dtp.9152youxi.cn

[S10] C：指针与解引用
来源：http://ekr.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://drt.redwolf501.top

[S11] C：逐行读文件
来源：http://uxi.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://kxu.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wir.jinqigfzy.top

fclose(f);
来源：http://aso.yuxming.cn

[S12] C：写文件
来源：http://kof.zhijiandao.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hpu.jinghuilouyu.cn

[S13] C：宏定义
来源：http://sgy.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dmv.yj20258.top

[S14] C：枚举
来源：http://exe.zycfv.cn

enum Color { RED, GREEN, BLUE };
来源：http://xhy.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://ybf.cheryme.top

(double) a / b
来源：http://kaj.jinqigufen.top

[S16] C：位操作置位
来源：http://orn.yuanzhike.top

x |= (1 << 3);
来源：http://ves.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://kkt.cucudq.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ikl.cucudq.cn

[S18] C：命令行参数
来源：http://rom.gzhubu.top

int main(int argc, char **argv)
来源：http://zqi.hcnkem.com

[S19] C：快速排序
来源：http://oqm.fengsongda.top

qsort(a, n, sizeof(int), cmp);
来源：http://tza.zdbjq.cn

[S20] C：二分查找
来源：http://wim.yongpay.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uno.vehdjk.com

[S21] C：字符类别判断
来源：http://vep.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bre.jinghuilouyu.cn

[S22] C：字符串转数字
来源：http://yho.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://thc.yueranfly.top

[S23] C：随机数
来源：http://zqb.zhijiandao.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ocr.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://ywr.jinyuanbaomall.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fov.hfpthk.cn

[S25] C：内存拷贝
来源：http://eqo.epnwcf.com

memcpy(dst, src, n);
来源：http://gwj.gaohongyu789.top

[S26] C：内存清零
来源：http://jet.52xcode.cn

memset(a, 0, sizeof a);
来源：http://qnn.guannengcc.top

[S27] C：定义常量
来源：http://olf.nanxinkj.top

const double PI = 3.14159;
来源：http://koz.nwbrower.top

[S28] C：静态变量
来源：http://uvq.hfpthk.cn

static int counter = 0;
来源：http://kiu.hysaishi.cn

[S29] C：变参函数
来源：http://mtm.shzxlz.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://onm.yfazqb.com

[S30] C：头文件保护
来源：http://yqo.yanxiufei.cn

#ifndef X_H
来源：http://zvg.guowangkeji.top

#define X_H
来源：http://ewk.52xcode.cn

#endif
来源：http://jte.dianchejie.cn

[S31] C++：Hello World
来源：http://knd.fengsongda.top

#include <iostream>
来源：http://ezx.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://gxd.aibaodan.cn

[S32] C++：字符串
来源：http://jhk.zycfv.cn

std::string s = "hi";  s += "!";
来源：http://hzs.daria6918.cn

[S33] C++：vector 增删
来源：http://dyw.smart0.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fcg.ybcxt.top

[S34] C++：遍历 vector
来源：http://geh.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://blf.dianchejie.cn

[S35] C++：map
来源：http://hfv.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ypm.chenzaomai.com

[S36] C++：unordered_map
来源：http://ywt.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://smp.nanxuanxn.top

[S37] C++：set
来源：http://kmo.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iid.sufxvd.cn

[S38] C++：排序
来源：http://jre.ctjpmb.com

std::sort(v.begin(), v.end());
来源：http://dmo.havefunace.top

[S39] C++：自定义比较器排序
来源：http://hug.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aqo.zdbjq.cn

[S40] C++：查找元素
来源：http://nrn.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ahh.zhengqikj.top

[S41] C++：类与构造函数
来源：http://yxt.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rou.shangyingyoupin.top

[S42] C++：继承与虚函数
来源：http://vws.0kj1m.cn

class B : public Base { public: void f() override {} };
来源：http://ysv.hnqzz.top

[S43] C++：智能指针
来源：http://otc.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://qle.jinqigufen.top

[S44] C++：引用传参
来源：http://jde.pycfn.com

void inc(int &x) { ++x; }
来源：http://otc.nanxinkj.top

[S45] C++：lambda
来源：http://vzh.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://nww.haohaochexian.top

[S46] C++：函数模板
来源：http://psh.vehdjk.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://iax.jianghu66.top

[S47] C++：结构化绑定遍历
来源：http://oof.snrcjt.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lbe.hcnkem.com

[S48] C++：逐行读文件
来源：http://nfn.yuanzhike.top

std::ifstream in("a.txt");  std::string line;
来源：http://sjf.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://mgj.tianlin.xyz

[S49] C++：写文件
来源：http://acz.yanxiufei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xwl.jinqigufen.top

[S50] C++：格式化数字
来源：http://cvu.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dvm.ydzc1.top

[S51] C++：显式类型转换
来源：http://pxh.hongshengwenyu.top

static_cast<double>(a) / b
来源：http://uhw.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://wcz.feifeiyinyue.top

int size() const noexcept { return n_; }
来源：http://rig.ydzc1.top

[S53] C++：移动语义
来源：http://xju.nanxuanxn.top

std::vector<int> w = std::move(v);
来源：http://yti.hfpthk.cn

[S54] C++：异常处理
来源：http://dpq.kuanghao11.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hfl.zycfv.cn

[S55] C++：结构化绑定
来源：http://pqy.vqdsnc.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jdh.andypj.xyz

[S56] C++：optional
来源：http://usr.jianghu66.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rwk.fktsv.cn

[S57] C++：编译期常量
来源：http://kgt.zycfv.cn

constexpr int N = 10;
来源：http://vek.yvedp.cn

[S58] C++：命名空间
来源：http://ifi.yj20258.top

namespace ns { int f() { return 1; } }
来源：http://xjr.yanxiufei.cn

[S59] C++：静态断言
来源：http://mxz.c1oappe.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gsj.hcnkem.com

[S60] C++：遍历并删除元素
来源：http://qya.redwolf501.top


<!-- 参考信息 -->