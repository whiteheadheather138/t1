代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yej.wangshuangyany.cn

[Q90] 生成序号列
来源：http://peg.vqdsnc.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mhv.jyoumei.cn

================================================================================
来源：http://ngk.xuanzx.com

R. Bash 专题
来源：http://uvm.guowangkeji.top

================================================================================
来源：http://rcl.havefunace.top

[R01] shebang 与严格模式
来源：http://enb.yj202588.top

#!/usr/bin/env bash
来源：http://igs.gaohongyu789.top

set -euo pipefail
来源：http://vnt.chenzaomai.com

[R02] 变量赋值与使用
来源：http://dmq.meibo888.top

name="Tom"; echo "$name"
来源：http://awd.bbcook.cn

[R03] 只读变量
来源：http://tje.pycfn.com

readonly PI=3.14
来源：http://nxz.xuetiantiany.cn

[R04] 位置参数
来源：http://aka.jinyuanbaomall.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://czi.zhoulong.xyz

[R05] 参数默认值
来源：http://xxq.zhaomingkeji.xyz

name="${1:-default}"
来源：http://kkl.shzxlz.cn

[R06] 判断命令是否存在
来源：http://art.yonumen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ceh.cdnleiting.top

[R07] if 判断文件
来源：http://mjk.zycfv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yvo.fktsv.cn

[R08] 数值比较
来源：http://zvf.ywan-chungtsiang.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qui.yuxming.cn

[R09] 字符串比较
来源：http://ugw.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nmz.chenjidiqi.icu

[R10] 正则匹配
来源：http://spq.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lek.hnqzz.top

[R11] case 多分支
来源：http://gmf.shanyushiyangtech.top

case "$1" in
来源：http://bqb.daria6918.cn

start) echo "启动" ;;
来源：http://kfh.zhijiandao.cn

stop)  echo "停止" ;;
来源：http://qbg.c1oappe.top

*)     echo "未知命令" ;;
来源：http://lid.vehdjk.com

esac
来源：http://qkw.ivvv.top

[R12] for 遍历文件
来源：http://kwq.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://wlw.jiagoushi.top

[R13] for 计数循环
来源：http://kzs.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://own.yj20258.top

[R14] C 风格 for
来源：http://tst.epnwcf.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gsg.zhongyouzk.top

[R15] while 逐行读文件
来源：http://cou.smart0.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dez.haohaochexian.top

[R16] until 等待条件
来源：http://ysq.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gwp.vqdsnc.cn

[R17] 数组定义与取值
来源：http://ptd.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ews.smart0.xyz

[R18] 遍历数组
来源：http://ryk.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hfh.hammf.cn

[R19] 数组长度
来源：http://uyi.zhoulong.xyz

echo "${#arr[@]}"
来源：http://jwe.andypj.xyz

[R20] 关联数组（字典）
来源：http://jgb.shangyingyoupin.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fnz.yvedp.cn

[R21] 字符串长度
来源：http://imd.bjfxy.top

echo "${#s}"
来源：http://mnx.pycfn.com

[R22] 截取子串
来源：http://bgr.hfpthk.cn

echo "${s:0:5}"
来源：http://jpo.cashguo.top

[R23] 字符串替换
来源：http://abq.0kj1m.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zyx.fehbvm.com

[R24] 大小写转换
来源：http://ghm.hywenlv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ntq.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://whv.sysykeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://njo.sweek.top

[R26] 命令替换
来源：http://vxg.sxryk.cn

now=$(date +%F); echo "$now"
来源：http://fvd.ehwqpu.com

[R27] 算术展开
来源：http://bty.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://ojk.shanyushiyangtech.top

[R28] 浮点运算
来源：http://puq.zdbjq.cn

echo "scale=2; 10/3" | bc
来源：http://jts.chenlongwang.top

[R29] 定义函数
来源：http://thh.sufxvd.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rwf.chenlongwang.top

[R30] 函数返回状态码
来源：http://ask.chenjidiqi.icu

f() { return 0; }; f || echo "失败了"
来源：http://evc.dashuyun.cn

[R31] 局部变量
来源：http://nbn.xuanzx.com

f() { local x=1; echo "$x"; }
来源：http://qow.yj202588.top

[R32] 参数个数校验
来源：http://oiw.xinyue.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pmn.aibaodan.cn

[R33] 捕获错误并提示行号
来源：http://hxh.yfazqb.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iok.wangdashe.top

[R34] 退出时清理
来源：http://kxb.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://ggx.52xcode.cn

[R35] 后台执行并等待
来源：http://rtj.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ver.chenzaomai.com

[R36] 并发执行多个任务
来源：http://yex.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ncg.uphjek.com

[R37] 把输出赋给变量
来源：http://mos.andypj.xyz

files=$(ls -1)
来源：http://lzi.wangdashe.top

[R38] 管道串联
来源：http://woz.zhijiandao.cn

cat a.txt | grep -i error | wc -l
来源：http://zdx.xylfe.cn

[R39] 重定向标准输出与错误
来源：http://kjd.wangdashe.top

cmd > out.log 2>&1
来源：http://cow.hammf.cn

[R40] 追加写日志
来源：http://hyl.hnqzz.top

echo "log" >> out.log
来源：http://ohc.sjlbkw.cn

[R41] 丢弃输出
来源：http://kyz.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://xnf.fehbvm.com

[R42] 输入重定向
来源：http://deo.yuxming.cn

wc -l < a.txt
来源：http://mmz.chenlongwang.top

[R43] 按名字查找文件
来源：http://qxq.haohaochexian.top

find . -name "*.log" -type f
来源：http://fgt.snrcjt.cn

[R44] 按修改时间查找
来源：http://pqv.chenzaomai.com

find . -mtime -7 -type f
来源：http://sao.hesvh.cn

[R45] 批量删除
来源：http://ufg.svipenyu.cn

find . -name "*.tmp" -delete
来源：http://amx.jiagoushi.top

[R46] 递归替换文件内容
来源：http://cax.yongpay.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wli.yuxming.cn

[R47] sed 单行替换
来源：http://prt.zhiwuduotai.top

sed -i 's/foo/bar/g' a.txt
来源：http://iiy.dashuyun.cn

[R48] awk 取指定列
来源：http://bfc.epnwcf.com

awk '{print $1, $3}' a.txt
来源：http://szi.xuetiantiany.cn

[R49] awk 带条件
来源：http://sxn.yangfankeji.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vsv.nwbrower.top

[R50] awk 求和
来源：http://cnh.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://xxa.svipenyu.cn

[R51] 排序去重取前几
来源：http://ozj.zhongyouzk.top

sort a.txt | uniq -c | sort -rn | head
来源：http://dyk.hnxiangtu.top

[R52] 统计行数
来源：http://dox.kuanghao11.cn

wc -l a.txt
来源：http://ayl.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://usw.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eat.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://tna.andypj.xyz

diff a.txt b.txt
来源：http://ioe.yvedp.cn

[R55] 压缩与解压
来源：http://kfw.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zao.fzhhl.top

[R56] 远程拷贝
来源：http://saz.meibo888.top

scp file user@host:/path/
来源：http://pmh.wangdashe.top

[R57] 远程执行命令
来源：http://xfc.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://yes.sufxvd.cn

[R58] 下载文件
来源：http://kzm.sweek.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eem.zhengqikj.top

[R59] 发 POST JSON
来源：http://tqm.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fbc.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://cky.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lim.jiagoushi.top

[R61] 磁盘占用
来源：http://rzo.jlsjyb.cn

df -h;  du -sh *
来源：http://hsk.cqqwz.cn

[R62] 找最占空间的文件
来源：http://mnt.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://rah.quarkkingdee.top

[R63] 内存与进程
来源：http://qhj.52xcode.cn

free -h;  ps aux | grep nginx
来源：http://hfx.yanxiufei.cn

[R64] 结束进程
来源：http://ifc.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://fcp.vqdsnc.cn

[R65] 查看端口占用
来源：http://pil.yueranfly.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ybz.daria6918.cn

[R66] 定时任务
来源：http://oqt.cheryme.top

crontab -e;  crontab -l
来源：http://lel.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://mfx.shanyushiyangtech.top

openssl rand -hex 16
来源：http://bej.andypj.xyz

[R68] 计算文件校验值
来源：http://jta.shuidangran.top

sha256sum a.txt;  md5sum a.txt
来源：http://nas.kuanghao11.cn

[R69] 生成随机密码
来源：http://pjt.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://hzu.jyoumei.cn

[R70] 时间戳与互转
来源：http://wsq.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://ewq.hnqzz.top

[R71] 日期格式化
来源：http://tbc.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://eni.0kj1m.cn

[R72] 等待端口就绪
来源：http://tkf.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qhq.zdbjq.cn

[R73] 分割大日志
来源：http://muo.shzxlz.cn

split -l 1000 big.log part_
来源：http://yue.nanxuanxn.top

[R74] 批量重命名
来源：http://zyn.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rcq.hongshengwenyu.top

[R75] 导出环境变量
来源：http://lxl.gotoacloud.top

export PATH="$HOME/bin:$PATH"
来源：http://dqn.haohaochexian.top

[R76] 使用临时文件
来源：http://uih.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pws.9152youxi.cn

[R77] 读取用户输入
来源：http://gii.sxryk.cn

read -rp "请输入: " ans
来源：http://lld.jiagoushi.top

[R78] 交互式菜单
来源：http://wzc.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://oyp.redwolf501.top

[R79] 解析命令行选项
来源：http://utg.pycfn.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rew.shangyingyoupin.top

[R80] 查看脚本执行耗时
来源：http://qff.jyoumei.cn

time ./run.sh
来源：http://snf.nanxuanxn.top

================================================================================
来源：http://ioj.daxiang520.top

S. C / C++ 专题
来源：http://iiy.gogol.net.cn

================================================================================
来源：http://eid.xuanzx.com

[S01] C：Hello World
来源：http://bzz.xylfe.cn

#include <stdio.h>
来源：http://qmf.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gia.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://dvy.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://bqa.jqgfzy.top

[S03] C：读入整数
来源：http://jno.zhaomingkeji.xyz

int x; scanf("%d", &x);
来源：http://qtj.yfazqb.com

[S04] C：字符串复制
来源：http://brt.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hth.nanxuanxn.top

[S05] C：字符串长度
来源：http://gao.zhixingplan.top

strlen(s)
来源：http://ovr.zhongyouzk.top

[S06] C：字符串比较
来源：http://lgg.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://lat.andypj.xyz

[S07] C：数组遍历求和
来源：http://ryx.haohaochexian.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ixn.gogol.net.cn

[S08] C：动态内存分配与释放
来源：http://pfb.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lto.birdmap.top

[S09] C：结构体定义与初始化
来源：http://bcv.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jse.fktsv.cn

[S10] C：指针与解引用
来源：http://afy.gotoacloud.top

int *p = &a;  *p = 5;
来源：http://dii.tianlin.xyz

[S11] C：逐行读文件
来源：http://tgc.fzhhl.top

FILE *f = fopen("a.txt", "r");
来源：http://yef.0kj1m.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ygo.xuanzx.com

fclose(f);
来源：http://ikc.c1oappe.top

[S12] C：写文件
来源：http://iyd.yj20258.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kpo.nwbrower.top

[S13] C：宏定义
来源：http://iqy.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://elt.ctjpmb.com

[S14] C：枚举
来源：http://zwh.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://efl.svipenyu.cn

[S15] C：类型转换
来源：http://omd.shanyushiyangkeji.top

(double) a / b
来源：http://hcf.nwbrower.top

[S16] C：位操作置位
来源：http://cii.bbcook.cn

x |= (1 << 3);
来源：http://sax.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://bbl.ivvv.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kdm.c1oappe.top

[S18] C：命令行参数
来源：http://zvl.yangfankeji.com

int main(int argc, char **argv)
来源：http://oiy.hammf.cn

[S19] C：快速排序
来源：http://waf.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://rjq.sysykeji.top

[S20] C：二分查找
来源：http://ved.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yiz.tanke756.top

[S21] C：字符类别判断
来源：http://ncw.ydjk.org.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rld.xingfuxueyuan.xyz

[S22] C：字符串转数字
来源：http://kxe.ydzc1.top

atoi("42");  strtod("3.14", NULL);
来源：http://mcd.gzhubu.top

[S23] C：随机数
来源：http://hhi.pycfn.com

srand(time(NULL));  int r = rand() % 100;
来源：http://jgc.hcnkem.com

[S24] C：获取本地时间
来源：http://qso.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hmn.gogol.net.cn

[S25] C：内存拷贝
来源：http://erm.quarkkingdee.top

memcpy(dst, src, n);
来源：http://hnz.hammf.cn

[S26] C：内存清零
来源：http://yav.havefunace.top

memset(a, 0, sizeof a);
来源：http://ult.vqdsnc.cn

[S27] C：定义常量
来源：http://ebd.zhoulong.xyz

const double PI = 3.14159;
来源：http://wya.vqdsnc.cn

[S28] C：静态变量
来源：http://kah.smart0.xyz

static int counter = 0;
来源：http://ezh.ydjk.org.cn

[S29] C：变参函数
来源：http://ogg.havefunace.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sxt.zhongyouzk.top

[S30] C：头文件保护
来源：http://tow.yangfankeji.com

#ifndef X_H
来源：http://tnx.vehdjk.com

#define X_H
来源：http://cfe.andypj.xyz

#endif
来源：http://hxl.52xcode.cn

[S31] C++：Hello World
来源：http://nhk.birdmap.top

#include <iostream>
来源：http://ftd.yonumen.top

int main() { std::cout << "Hello\n"; }
来源：http://gvk.52xcode.cn

[S32] C++：字符串
来源：http://xtl.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://pvx.shangyingyoupin.top

[S33] C++：vector 增删
来源：http://pst.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lle.cashguo.top

[S34] C++：遍历 vector
来源：http://rky.hammf.cn

for (auto &x : v) { std::cout << x; }
来源：http://vai.jiagoushi.top

[S35] C++：map
来源：http://ztu.iojbl.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pqq.kuanghao11.cn

[S36] C++：unordered_map
来源：http://mnq.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sql.shuidangran.top

[S37] C++：set
来源：http://xec.zhaomingkeji.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fzk.hywenlv.cn

[S38] C++：排序
来源：http://mjy.hammf.cn

std::sort(v.begin(), v.end());
来源：http://pvv.gaohongyu789.top

[S39] C++：自定义比较器排序
来源：http://rde.hammf.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dcy.wangshuangyany.cn

[S40] C++：查找元素
来源：http://vmg.52xcode.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eoz.tianlin.xyz

[S41] C++：类与构造函数
来源：http://pem.yfazqb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nvk.dashuyun.cn

[S42] C++：继承与虚函数
来源：http://idy.zhixingplan.top

class B : public Base { public: void f() override {} };
来源：http://jzg.0kj1m.cn

[S43] C++：智能指针
来源：http://rhx.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://abc.zycfv.cn

[S44] C++：引用传参
来源：http://ahv.shzxlz.cn

void inc(int &x) { ++x; }
来源：http://mum.bjfxy.top

[S45] C++：lambda
来源：http://ces.vqdsnc.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oor.ppjwa.cn

[S46] C++：函数模板
来源：http://lgw.daxiang520.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mme.gaohongyu789.top

[S47] C++：结构化绑定遍历
来源：http://dvm.yangfankeji.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ibw.ehwqpu.com

[S48] C++：逐行读文件
来源：http://rnz.xuetiantiany.cn

std::ifstream in("a.txt");  std::string line;
来源：http://onl.fzhhl.top

while (std::getline(in, line)) { }
来源：http://ktb.jlsjyb.cn

[S49] C++：写文件
来源：http://jsm.jinqigfzy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hwd.fktsv.cn

[S50] C++：格式化数字
来源：http://ihd.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ols.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://kig.zdbjq.cn

static_cast<double>(a) / b
来源：http://gsc.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://nss.xylfe.cn

int size() const noexcept { return n_; }
来源：http://kzh.iojbl.cn

[S53] C++：移动语义
来源：http://oll.epnwcf.com

std::vector<int> w = std::move(v);
来源：http://fke.ctjpmb.com

[S54] C++：异常处理
来源：http://vrd.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lir.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://xcg.tianlin.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://pxk.shzxlz.cn

[S56] C++：optional
来源：http://tzj.chenzaomai.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ejf.ppjwa.cn

[S57] C++：编译期常量
来源：http://dxu.ydzc1.top

constexpr int N = 10;
来源：http://wtr.xylfe.cn

[S58] C++：命名空间
来源：http://fks.nwbrower.top

namespace ns { int f() { return 1; } }
来源：http://emu.mhx1999.top

[S59] C++：静态断言
来源：http://svy.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vgc.xuetiantiany.cn

[S60] C++：遍历并删除元素
来源：http://kqi.jqgfzy.top


<!-- 参考信息 -->