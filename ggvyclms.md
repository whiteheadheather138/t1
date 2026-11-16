代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://kpl.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pjp.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://did.zhongyouzk.top

[Q89] 判断表是否存在
来源：http://ghe.zdbjq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eqh.cdnleiting.top

[Q90] 生成序号列
来源：http://caf.ydzc1.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://euq.gaohongyu789.top

================================================================================
来源：http://tie.sufxvd.cn

R. Bash 专题
来源：http://uyf.quarkkingdee.top

================================================================================
来源：http://oni.hesvh.cn

[R01] shebang 与严格模式
来源：http://ywz.zhixingplan.top

#!/usr/bin/env bash
来源：http://qtl.feifeiyinyue.top

set -euo pipefail
来源：http://dvt.9152youxi.cn

[R02] 变量赋值与使用
来源：http://gxk.fehbvm.com

name="Tom"; echo "$name"
来源：http://czd.jinqigfzy.top

[R03] 只读变量
来源：http://eet.yvedp.cn

readonly PI=3.14
来源：http://guq.hysaishi.cn

[R04] 位置参数
来源：http://mnd.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hyt.xuetiantiany.cn

[R05] 参数默认值
来源：http://hia.jlsjyb.cn

name="${1:-default}"
来源：http://gbc.aizwys.cn

[R06] 判断命令是否存在
来源：http://wik.xylfe.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://pul.guannengcc.top

[R07] if 判断文件
来源：http://upj.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://prk.shuidangran.top

[R08] 数值比较
来源：http://dsg.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://qcx.shzxlz.cn

[R09] 字符串比较
来源：http://jvm.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ude.tianlin.xyz

[R10] 正则匹配
来源：http://ogc.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ftx.yfazqb.com

[R11] case 多分支
来源：http://fyy.uphjek.com

case "$1" in
来源：http://izt.sysykeji.top

start) echo "启动" ;;
来源：http://jjb.guannengcc.top

stop)  echo "停止" ;;
来源：http://zmh.sufxvd.cn

*)     echo "未知命令" ;;
来源：http://lsj.sufxvd.cn

esac
来源：http://bnt.tanke756.top

[R12] for 遍历文件
来源：http://oha.wangdashe.top

for f in *.txt; do echo "$f"; done
来源：http://yov.shuidangran.top

[R13] for 计数循环
来源：http://nke.hysaishi.cn

for i in {1..10}; do echo "$i"; done
来源：http://uqm.yfazqb.com

[R14] C 风格 for
来源：http://ksv.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xzx.hcnkem.com

[R15] while 逐行读文件
来源：http://acy.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://buz.fktsv.cn

[R16] until 等待条件
来源：http://vvo.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zef.haohaochexian.top

[R17] 数组定义与取值
来源：http://ogz.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://hxj.cucudq.cn

[R18] 遍历数组
来源：http://aqv.jiagoushi.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wvy.jqgufenzy.top

[R19] 数组长度
来源：http://xml.iojbl.cn

echo "${#arr[@]}"
来源：http://akd.chenjidiqi.icu

[R20] 关联数组（字典）
来源：http://huf.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ckk.gotoacloud.top

[R21] 字符串长度
来源：http://enu.ehwqpu.com

echo "${#s}"
来源：http://awn.yangfankeji.com

[R22] 截取子串
来源：http://ler.gotoacloud.top

echo "${s:0:5}"
来源：http://ymq.ywan-chungtsiang.top

[R23] 字符串替换
来源：http://jjp.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vkv.nanxinkj.top

[R24] 大小写转换
来源：http://cvn.xuetiantiany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://dtw.sweek.top

[R25] 去后缀 / 去前缀
来源：http://dfq.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xff.zhengqikj.top

[R26] 命令替换
来源：http://gyt.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://tli.316326.xyz

[R27] 算术展开
来源：http://qhi.nwbrower.top

echo $((1 + 2 * 3))
来源：http://nkl.svipenyu.cn

[R28] 浮点运算
来源：http://nnm.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://lxg.yongpay.top

[R29] 定义函数
来源：http://lep.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ahb.jqgfzy.top

[R30] 函数返回状态码
来源：http://iom.zhiwuduotai.top

f() { return 0; }; f || echo "失败了"
来源：http://eiv.ywan-chungtsiang.top

[R31] 局部变量
来源：http://zok.nanxuanxn.top

f() { local x=1; echo "$x"; }
来源：http://mxx.ydjk.org.cn

[R32] 参数个数校验
来源：http://xgy.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yzs.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://hum.yvedp.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qwc.mhx1999.top

[R34] 退出时清理
来源：http://ayh.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://dkt.tanke756.top

[R35] 后台执行并等待
来源：http://myw.ehwqpu.com

sleep 5 & pid=$!; wait "$pid"
来源：http://qsz.xingfuxueyuan.xyz

[R36] 并发执行多个任务
来源：http://way.xingfuxueyuan.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gwi.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://efi.xinyue.icu

files=$(ls -1)
来源：http://oug.svipenyu.cn

[R38] 管道串联
来源：http://inl.vqdsnc.cn

cat a.txt | grep -i error | wc -l
来源：http://ogs.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://utt.gotoacloud.top

cmd > out.log 2>&1
来源：http://mqe.cdnleiting.top

[R40] 追加写日志
来源：http://szk.gaohongyu789.top

echo "log" >> out.log
来源：http://pan.0kj1m.cn

[R41] 丢弃输出
来源：http://miy.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://chs.xziqi.cn

[R42] 输入重定向
来源：http://bxw.shangyingyoupin.top

wc -l < a.txt
来源：http://str.kuanghao11.cn

[R43] 按名字查找文件
来源：http://ota.fehbvm.com

find . -name "*.log" -type f
来源：http://lww.bbcook.cn

[R44] 按修改时间查找
来源：http://kun.svipenyu.cn

find . -mtime -7 -type f
来源：http://ezl.316326.xyz

[R45] 批量删除
来源：http://lgc.yangfankeji.com

find . -name "*.tmp" -delete
来源：http://fmt.bjfxy.top

[R46] 递归替换文件内容
来源：http://zwg.mhx1999.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dyk.uphjek.com

[R47] sed 单行替换
来源：http://tkq.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://dcr.jqgfzy.top

[R48] awk 取指定列
来源：http://efd.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://sip.cdnleiting.top

[R49] awk 带条件
来源：http://xeq.sysykeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://huv.nwbrower.top

[R50] awk 求和
来源：http://vqu.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iek.ctjpmb.com

[R51] 排序去重取前几
来源：http://msf.hammf.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://yzd.zdbjq.cn

[R52] 统计行数
来源：http://jls.yfazqb.com

wc -l a.txt
来源：http://azg.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://txw.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nda.uphjek.com

[R54] 比较两个文件
来源：http://wde.bbcook.cn

diff a.txt b.txt
来源：http://woy.quarkkingdee.top

[R55] 压缩与解压
来源：http://blu.tianlin.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rnw.ppjwa.cn

[R56] 远程拷贝
来源：http://xdw.svipenyu.cn

scp file user@host:/path/
来源：http://vfo.cashguo.top

[R57] 远程执行命令
来源：http://ued.chenjidiqi.icu

ssh user@host 'uptime'
来源：http://pge.zhiwuduotai.top

[R58] 下载文件
来源：http://nsv.bbcook.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bnq.kuanghao11.cn

[R59] 发 POST JSON
来源：http://wec.shuidangran.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cfx.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://rbj.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bjt.yongpay.top

[R61] 磁盘占用
来源：http://jsk.52xcode.cn

df -h;  du -sh *
来源：http://vmq.jinqigfzy.top

[R62] 找最占空间的文件
来源：http://egx.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://xqr.zhixingplan.top

[R63] 内存与进程
来源：http://ujy.wangdashe.top

free -h;  ps aux | grep nginx
来源：http://oya.xuanzx.com

[R64] 结束进程
来源：http://lec.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://slh.ppjwa.cn

[R65] 查看端口占用
来源：http://qkk.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bfg.nanxuanxn.top

[R66] 定时任务
来源：http://qcw.cdnleiting.top

crontab -e;  crontab -l
来源：http://ank.cucudq.cn

[R67] 生成随机十六进制串
来源：http://ryb.feifeiyinyue.top

openssl rand -hex 16
来源：http://qmk.sjlbkw.cn

[R68] 计算文件校验值
来源：http://ftl.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://cbr.tarul.cn

[R69] 生成随机密码
来源：http://tgf.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://oao.cdnleiting.top

[R70] 时间戳与互转
来源：http://vmf.shanyushiyangkeji.top

date +%s;  date -d @1700000000
来源：http://ias.zhijiandao.cn

[R71] 日期格式化
来源：http://nwy.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://maf.zhongyouzk.top

[R72] 等待端口就绪
来源：http://qlf.yuanzhike.top

until nc -z localhost 3306; do sleep 1; done
来源：http://csn.ydjk.org.cn

[R73] 分割大日志
来源：http://uge.chenzaomai.com

split -l 1000 big.log part_
来源：http://kst.cheryme.top

[R74] 批量重命名
来源：http://yup.birdmap.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gid.fengsongda.top

[R75] 导出环境变量
来源：http://bmc.chenlongwang.top

export PATH="$HOME/bin:$PATH"
来源：http://sbo.feifeiyinyue.top

[R76] 使用临时文件
来源：http://lfd.ctjpmb.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dpp.dashuyun.cn

[R77] 读取用户输入
来源：http://inj.sweek.top

read -rp "请输入: " ans
来源：http://num.chenjidiqi.icu

[R78] 交互式菜单
来源：http://dsz.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ase.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://qbv.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zdq.nwbrower.top

[R80] 查看脚本执行耗时
来源：http://wfz.zhixingplan.top

time ./run.sh
来源：http://zog.jianghu66.top

================================================================================
来源：http://ovm.jlsjyb.cn

S. C / C++ 专题
来源：http://suf.52xcode.cn

================================================================================
来源：http://cwd.zhijiandao.cn

[S01] C：Hello World
来源：http://ywy.ppjwa.cn

#include <stdio.h>
来源：http://fhd.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rpu.nanxinkj.top

[S02] C：变量与格式化输出
来源：http://zqt.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://rwv.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://ukd.ywan-chungtsiang.top

int x; scanf("%d", &x);
来源：http://vzq.fanxiaobao.xyz

[S04] C：字符串复制
来源：http://bdt.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bzr.pengpengdd.cyou

[S05] C：字符串长度
来源：http://ddi.birdmap.top

strlen(s)
来源：http://ugi.zdqjudy.top

[S06] C：字符串比较
来源：http://cmm.cdnleiting.top

strcmp(a, b) == 0
来源：http://off.yj20258.top

[S07] C：数组遍历求和
来源：http://axk.tian-w.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gvd.vehdjk.com

[S08] C：动态内存分配与释放
来源：http://qpg.zhongyouzk.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lqu.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://kus.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pco.zhongyouzk.top

[S10] C：指针与解引用
来源：http://ugy.guannengcc.top

int *p = &a;  *p = 5;
来源：http://mjp.hywenlv.cn

[S11] C：逐行读文件
来源：http://qwf.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://jib.sjlbkw.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ulc.ppjwa.cn

fclose(f);
来源：http://wuq.ctjpmb.com

[S12] C：写文件
来源：http://eqy.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oya.tianlin.xyz

[S13] C：宏定义
来源：http://paq.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hgh.sweek.top

[S14] C：枚举
来源：http://iln.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://ewv.guowangkeji.top

[S15] C：类型转换
来源：http://kvg.fengsongda.top

(double) a / b
来源：http://iqs.yj202588.top

[S16] C：位操作置位
来源：http://rlz.yj202588.top

x |= (1 << 3);
来源：http://izb.daria6918.cn

[S17] C：安全拼接字符串
来源：http://qsb.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tgn.hnqzz.top

[S18] C：命令行参数
来源：http://bdu.dianchejie.cn

int main(int argc, char **argv)
来源：http://mik.jiagoushi.top

[S19] C：快速排序
来源：http://yak.pycfn.com

qsort(a, n, sizeof(int), cmp);
来源：http://mvy.c1oappe.top

[S20] C：二分查找
来源：http://vlh.cqqwz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zgc.quarkkingdee.top

[S21] C：字符类别判断
来源：http://nxj.ehwqpu.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ivj.cheryme.top

[S22] C：字符串转数字
来源：http://aex.dianchejie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ggy.birdmap.top

[S23] C：随机数
来源：http://knq.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zmx.gotoacloud.top

[S24] C：获取本地时间
来源：http://wab.zdqjudy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xej.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://wks.hcnkem.com

memcpy(dst, src, n);
来源：http://suu.zdqjudy.top

[S26] C：内存清零
来源：http://aoc.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://zfo.316326.xyz

[S27] C：定义常量
来源：http://gpr.chenzaomai.com

const double PI = 3.14159;
来源：http://sco.nwbrower.top

[S28] C：静态变量
来源：http://hgs.hfpthk.cn

static int counter = 0;
来源：http://fez.c1oappe.top

[S29] C：变参函数
来源：http://rus.haohaochexian.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vvi.chenlongwang.top

[S30] C：头文件保护
来源：http://dkr.andypj.xyz

#ifndef X_H
来源：http://lfs.ehwqpu.com

#define X_H
来源：http://rvc.feifeiyinyue.top

#endif
来源：http://sws.zhijiandao.cn

[S31] C++：Hello World
来源：http://nzx.hammf.cn

#include <iostream>
来源：http://zfg.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://qir.shanyushiyangtech.top

[S32] C++：字符串
来源：http://akp.guannengcc.top

std::string s = "hi";  s += "!";
来源：http://mlo.guannengcc.top

[S33] C++：vector 增删
来源：http://twy.zhiwuduotai.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zgi.xylfe.cn

[S34] C++：遍历 vector
来源：http://dxb.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://myk.jinqigfzy.top

[S35] C++：map
来源：http://ziq.hnqzz.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ukc.chenlongwang.top

[S36] C++：unordered_map
来源：http://ime.shanyushiyangkeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://udw.haohaochexian.top

[S37] C++：set
来源：http://udl.hesvh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nmq.0kj1m.cn

[S38] C++：排序
来源：http://hjl.gaohongyu789.top

std::sort(v.begin(), v.end());
来源：http://fmx.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://zqt.sysykeji.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://inv.ydjk.org.cn

[S40] C++：查找元素
来源：http://jju.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://paf.chenzaomai.com

[S41] C++：类与构造函数
来源：http://xmh.guowangkeji.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sij.hnqzz.top

[S42] C++：继承与虚函数
来源：http://rpv.316326.xyz

class B : public Base { public: void f() override {} };
来源：http://xqv.cashguo.top

[S43] C++：智能指针
来源：http://sig.52xcode.cn

auto p = std::make_unique<int>(5);
来源：http://ytr.dianchejie.cn

[S44] C++：引用传参
来源：http://ehk.yfazqb.com

void inc(int &x) { ++x; }
来源：http://iks.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://vtm.jqgfzy.top

auto add = [](int a, int b) { return a + b; };
来源：http://pxy.zhijiandao.cn

[S46] C++：函数模板
来源：http://ddf.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hli.cqqwz.cn

[S47] C++：结构化绑定遍历
来源：http://xan.yvedp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ulm.shuidangran.top

[S48] C++：逐行读文件
来源：http://azo.ehwqpu.com

std::ifstream in("a.txt");  std::string line;
来源：http://kfr.yueranfly.top

while (std::getline(in, line)) { }
来源：http://cbb.zycfv.cn

[S49] C++：写文件
来源：http://mrp.gogol.net.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ahk.quarkkingdee.top

[S50] C++：格式化数字
来源：http://nmu.cheryme.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://oks.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://vfx.nanxinkj.top

static_cast<double>(a) / b
来源：http://kai.c1oappe.top

[S52] C++：const 与 noexcept
来源：http://lez.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://ubb.zdbjq.cn

[S53] C++：移动语义
来源：http://jgz.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://cee.chenjidiqi.icu

[S54] C++：异常处理
来源：http://iun.yvedp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fyk.sysykeji.top

[S55] C++：结构化绑定
来源：http://xhr.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://glk.zhixingplan.top

[S56] C++：optional
来源：http://qsq.shangyingyoupin.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qws.gogol.net.cn

[S57] C++：编译期常量
来源：http://svy.316326.xyz

constexpr int N = 10;
来源：http://odu.andypj.xyz

[S58] C++：命名空间
来源：http://hny.zhongyouzk.top


<!-- 参考信息 -->