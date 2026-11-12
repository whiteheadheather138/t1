代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://tft.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gqk.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pqq.jqgfzy.top

[Q89] 判断表是否存在
来源：http://ijx.aizwys.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zfv.zhixingplan.top

[Q90] 生成序号列
来源：http://sxh.xuetiantiany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vzo.redwolf501.top

================================================================================
来源：http://ixg.fengsongda.top

R. Bash 专题
来源：http://zpj.shangyingyoupin.top

================================================================================
来源：http://wlc.zycfv.cn

[R01] shebang 与严格模式
来源：http://ybf.fengsongda.top

#!/usr/bin/env bash
来源：http://zey.hywenlv.cn

set -euo pipefail
来源：http://enz.yvedp.cn

[R02] 变量赋值与使用
来源：http://pvb.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://qqf.tarul.cn

[R03] 只读变量
来源：http://ucz.jinghuilouyu.cn

readonly PI=3.14
来源：http://rgk.9152youxi.cn

[R04] 位置参数
来源：http://tkb.yangfankeji.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yvs.shangyingyoupin.top

[R05] 参数默认值
来源：http://xtl.aizwys.cn

name="${1:-default}"
来源：http://fjh.yj20258.top

[R06] 判断命令是否存在
来源：http://cpo.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ppl.epnwcf.com

[R07] if 判断文件
来源：http://xfg.hnqzz.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://boe.nanxinkj.top

[R08] 数值比较
来源：http://grk.ctjpmb.com

if (( a > b )); then echo "a 更大"; fi
来源：http://smy.birdmap.top

[R09] 字符串比较
来源：http://lcu.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://the.kuanghao11.cn

[R10] 正则匹配
来源：http://xwj.nanxuanxn.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://chx.hesvh.cn

[R11] case 多分支
来源：http://kaz.gogol.net.cn

case "$1" in
来源：http://htn.gotoacloud.top

start) echo "启动" ;;
来源：http://qar.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://pei.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://djb.jinyuanbaomall.cn

esac
来源：http://uvq.hfpthk.cn

[R12] for 遍历文件
来源：http://ngx.smart0.xyz

for f in *.txt; do echo "$f"; done
来源：http://aci.shuidangran.top

[R13] for 计数循环
来源：http://gvr.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://asm.hfpthk.cn

[R14] C 风格 for
来源：http://ifr.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uen.yuxming.cn

[R15] while 逐行读文件
来源：http://dyn.yueranfly.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lor.zhaomingkeji.xyz

[R16] until 等待条件
来源：http://lih.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wxx.chenlongwang.top

[R17] 数组定义与取值
来源：http://yzc.shanyushiyangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://ygz.cashguo.top

[R18] 遍历数组
来源：http://web.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sse.nanxinkj.top

[R19] 数组长度
来源：http://mck.yfazqb.com

echo "${#arr[@]}"
来源：http://jnf.ivvv.top

[R20] 关联数组（字典）
来源：http://lgp.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zbw.xuetiantiany.cn

[R21] 字符串长度
来源：http://cup.sufxvd.cn

echo "${#s}"
来源：http://iej.guowangkeji.top

[R22] 截取子串
来源：http://llh.dianchejie.cn

echo "${s:0:5}"
来源：http://smd.snrcjt.cn

[R23] 字符串替换
来源：http://jgf.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lop.wangdashe.top

[R24] 大小写转换
来源：http://evg.jianghu66.top

echo "${s^^}"; echo "${s,,}"
来源：http://kzn.sweek.top

[R25] 去后缀 / 去前缀
来源：http://crg.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vlh.shzxlz.cn

[R26] 命令替换
来源：http://fvk.ywan-chungtsiang.top

now=$(date +%F); echo "$now"
来源：http://nrj.fengsongda.top

[R27] 算术展开
来源：http://lht.yuanzhike.top

echo $((1 + 2 * 3))
来源：http://tly.hywenlv.cn

[R28] 浮点运算
来源：http://bdh.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://adz.cqqwz.cn

[R29] 定义函数
来源：http://fou.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kfy.sysykeji.top

[R30] 函数返回状态码
来源：http://evu.hysaishi.cn

f() { return 0; }; f || echo "失败了"
来源：http://cwh.meibo888.top

[R31] 局部变量
来源：http://aar.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://fps.yongpay.top

[R32] 参数个数校验
来源：http://tsq.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yyn.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://jkb.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tbj.chenjidiqi.icu

[R34] 退出时清理
来源：http://wxj.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hwz.tarul.cn

[R35] 后台执行并等待
来源：http://sgr.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://emr.hysaishi.cn

[R36] 并发执行多个任务
来源：http://nrg.chenjidiqi.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://imt.hnqzz.top

[R37] 把输出赋给变量
来源：http://uyq.zhixingplan.top

files=$(ls -1)
来源：http://aym.bbcook.cn

[R38] 管道串联
来源：http://dby.feifeiyinyue.top

cat a.txt | grep -i error | wc -l
来源：http://pfn.hcnkem.com

[R39] 重定向标准输出与错误
来源：http://spb.gzhubu.top

cmd > out.log 2>&1
来源：http://glw.snrcjt.cn

[R40] 追加写日志
来源：http://ivt.cashguo.top

echo "log" >> out.log
来源：http://mcu.wangshuangyany.cn

[R41] 丢弃输出
来源：http://gxy.cheryme.top

cmd >/dev/null 2>&1
来源：http://kwx.fzhhl.top

[R42] 输入重定向
来源：http://fgw.jinqigfzy.top

wc -l < a.txt
来源：http://lrw.yonumen.top

[R43] 按名字查找文件
来源：http://gzw.nanxuanxn.top

find . -name "*.log" -type f
来源：http://lep.xinyue.icu

[R44] 按修改时间查找
来源：http://ybf.hesvh.cn

find . -mtime -7 -type f
来源：http://nur.jqgfzy.top

[R45] 批量删除
来源：http://sln.dianchejie.cn

find . -name "*.tmp" -delete
来源：http://gpw.jyoumei.cn

[R46] 递归替换文件内容
来源：http://omw.xuetiantiany.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jhb.kuanghao11.cn

[R47] sed 单行替换
来源：http://opu.nanxinkj.top

sed -i 's/foo/bar/g' a.txt
来源：http://fpc.jinyuanbaomall.cn

[R48] awk 取指定列
来源：http://fau.hysaishi.cn

awk '{print $1, $3}' a.txt
来源：http://vdw.jianghu66.top

[R49] awk 带条件
来源：http://bxr.ydzc1.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sed.hammf.cn

[R50] awk 求和
来源：http://kno.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://boy.hysaishi.cn

[R51] 排序去重取前几
来源：http://aqq.hcnkem.com

sort a.txt | uniq -c | sort -rn | head
来源：http://wtr.jinqigufen.top

[R52] 统计行数
来源：http://kaj.hammf.cn

wc -l a.txt
来源：http://otp.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://ejo.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tqv.yfazqb.com

[R54] 比较两个文件
来源：http://rns.yongpay.top

diff a.txt b.txt
来源：http://aod.shuidangran.top

[R55] 压缩与解压
来源：http://ndm.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://snx.fzhhl.top

[R56] 远程拷贝
来源：http://uds.feifeiyinyue.top

scp file user@host:/path/
来源：http://prk.ehwqpu.com

[R57] 远程执行命令
来源：http://byf.fanxiaobao.xyz

ssh user@host 'uptime'
来源：http://fgc.ivvv.top

[R58] 下载文件
来源：http://rui.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xgr.jianghu66.top

[R59] 发 POST JSON
来源：http://ybt.sxryk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gvg.jinyuanbaomall.cn

[R60] 只看 HTTP 状态码
来源：http://eio.hcnkem.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jfa.yueranfly.top

[R61] 磁盘占用
来源：http://nmd.smart0.xyz

df -h;  du -sh *
来源：http://ymd.tanke756.top

[R62] 找最占空间的文件
来源：http://ldw.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://vlp.andypj.xyz

[R63] 内存与进程
来源：http://yrc.fehbvm.com

free -h;  ps aux | grep nginx
来源：http://qcn.nwbrower.top

[R64] 结束进程
来源：http://gxx.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://xiz.cashguo.top

[R65] 查看端口占用
来源：http://osp.sxryk.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hij.zhengqikj.top

[R66] 定时任务
来源：http://nkw.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://jtp.cheryme.top

[R67] 生成随机十六进制串
来源：http://qbu.sufxvd.cn

openssl rand -hex 16
来源：http://vnl.meibo888.top

[R68] 计算文件校验值
来源：http://eyx.zdqjudy.top

sha256sum a.txt;  md5sum a.txt
来源：http://dlr.c1oappe.top

[R69] 生成随机密码
来源：http://kak.guannengcc.top

head -c 16 /dev/urandom | base64
来源：http://lry.guannengcc.top

[R70] 时间戳与互转
来源：http://owe.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://yuf.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://vem.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://fvi.andypj.xyz

[R72] 等待端口就绪
来源：http://kpb.hnqzz.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jle.hongshengwenyu.top

[R73] 分割大日志
来源：http://ssy.fktsv.cn

split -l 1000 big.log part_
来源：http://cie.aibaodan.cn

[R74] 批量重命名
来源：http://iuk.guannengcc.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rct.quarkkingdee.top

[R75] 导出环境变量
来源：http://kzg.fzhhl.top

export PATH="$HOME/bin:$PATH"
来源：http://zwp.meibo888.top

[R76] 使用临时文件
来源：http://mpo.fengsongda.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qjo.fktsv.cn

[R77] 读取用户输入
来源：http://ghk.cheryme.top

read -rp "请输入: " ans
来源：http://tts.yongpay.top

[R78] 交互式菜单
来源：http://nfk.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xmq.yanxiufei.cn

[R79] 解析命令行选项
来源：http://urf.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mzz.yj202588.top

[R80] 查看脚本执行耗时
来源：http://ppm.hfpthk.cn

time ./run.sh
来源：http://ytt.fengsongda.top

================================================================================
来源：http://yli.yj20258888.top

S. C / C++ 专题
来源：http://uzw.cashguo.top

================================================================================
来源：http://ebf.yfazqb.com

[S01] C：Hello World
来源：http://pjd.nanxinkj.top

#include <stdio.h>
来源：http://ymp.c1oappe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://mgi.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://wzy.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://ymx.shuidangran.top

[S03] C：读入整数
来源：http://phx.wangshuangyany.cn

int x; scanf("%d", &x);
来源：http://uxo.bjfxy.top

[S04] C：字符串复制
来源：http://bpl.zhiwuduotai.top

char dst[32]; strcpy(dst, "hi");
来源：http://tbv.vqdsnc.cn

[S05] C：字符串长度
来源：http://foj.yueranfly.top

strlen(s)
来源：http://gof.nwbrower.top

[S06] C：字符串比较
来源：http://buu.meibo888.top

strcmp(a, b) == 0
来源：http://trn.wangdashe.top

[S07] C：数组遍历求和
来源：http://koy.sjlbkw.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://drg.yangfankeji.com

[S08] C：动态内存分配与释放
来源：http://jan.zhixingplan.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://njg.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://abi.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oxa.bjfxy.top

[S10] C：指针与解引用
来源：http://ftv.gzhubu.top

int *p = &a;  *p = 5;
来源：http://wqv.wangshuangyany.cn

[S11] C：逐行读文件
来源：http://anr.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://hdi.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uxg.shzxlz.cn

fclose(f);
来源：http://rhn.yonumen.top

[S12] C：写文件
来源：http://fpg.iojbl.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bsc.yongpay.top

[S13] C：宏定义
来源：http://hnd.hcnkem.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ooc.ybcxt.top

[S14] C：枚举
来源：http://dcj.sjlbkw.cn

enum Color { RED, GREEN, BLUE };
来源：http://zob.hongshengwenyu.top

[S15] C：类型转换
来源：http://qsi.ydjk.org.cn

(double) a / b
来源：http://fjr.havefunace.top

[S16] C：位操作置位
来源：http://mqb.yvedp.cn

x |= (1 << 3);
来源：http://kwc.cheryme.top

[S17] C：安全拼接字符串
来源：http://rjm.hysaishi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jyx.feifeiyinyue.top

[S18] C：命令行参数
来源：http://lrt.zdbjq.cn

int main(int argc, char **argv)
来源：http://uup.zhixingplan.top

[S19] C：快速排序
来源：http://wng.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xfu.chenlongwang.top

[S20] C：二分查找
来源：http://jtq.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bkp.yvedp.cn

[S21] C：字符类别判断
来源：http://hyu.zhaomingkeji.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oud.ivvv.top

[S22] C：字符串转数字
来源：http://gnp.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nvn.zdqjudy.top

[S23] C：随机数
来源：http://jil.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oqo.ydzc1.top

[S24] C：获取本地时间
来源：http://ptw.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pfj.hesvh.cn

[S25] C：内存拷贝
来源：http://qlf.wangdashe.top

memcpy(dst, src, n);
来源：http://xwk.dianchejie.cn

[S26] C：内存清零
来源：http://mrk.zycfv.cn

memset(a, 0, sizeof a);
来源：http://kqn.uphjek.com

[S27] C：定义常量
来源：http://uje.zdbjq.cn

const double PI = 3.14159;
来源：http://udn.chenjidiqi.icu

[S28] C：静态变量
来源：http://ser.gogol.net.cn

static int counter = 0;
来源：http://ygu.ppjwa.cn

[S29] C：变参函数
来源：http://udv.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bfg.bbcook.cn

[S30] C：头文件保护
来源：http://lre.snrcjt.cn

#ifndef X_H
来源：http://vok.yangfankeji.com

#define X_H
来源：http://mub.sysykeji.top

#endif
来源：http://xbc.andypj.xyz

[S31] C++：Hello World
来源：http://wss.wangdashe.top

#include <iostream>
来源：http://gmp.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://pga.kuanghao11.cn

[S32] C++：字符串
来源：http://hkh.zhixingplan.top

std::string s = "hi";  s += "!";
来源：http://noz.nwbrower.top

[S33] C++：vector 增删
来源：http://drn.wangshuangyany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dda.snrcjt.cn

[S34] C++：遍历 vector
来源：http://dqh.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://wsb.chenjidiqi.icu

[S35] C++：map
来源：http://qtb.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uhc.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://gzr.nwbrower.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wiz.pycfn.com

[S37] C++：set
来源：http://flm.52xcode.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dzc.zhoulong.xyz

[S38] C++：排序
来源：http://acq.guannengcc.top

std::sort(v.begin(), v.end());
来源：http://pjd.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://xyp.jqgfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hiu.aibaodan.cn

[S40] C++：查找元素
来源：http://qoy.dashuyun.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vco.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://bnl.0kj1m.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ukw.iojbl.cn

[S42] C++：继承与虚函数
来源：http://wpw.xziqi.cn

class B : public Base { public: void f() override {} };
来源：http://jxr.iojbl.cn

[S43] C++：智能指针
来源：http://dpk.birdmap.top

auto p = std::make_unique<int>(5);
来源：http://cbb.quarkkingdee.top

[S44] C++：引用传参
来源：http://qyb.tian-w.cn

void inc(int &x) { ++x; }
来源：http://dvb.yj202588.top

[S45] C++：lambda
来源：http://mrb.jianghu66.top

auto add = [](int a, int b) { return a + b; };
来源：http://bgl.chenjidiqi.icu

[S46] C++：函数模板
来源：http://sqj.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gxf.xinyue.icu

[S47] C++：结构化绑定遍历
来源：http://tfq.gogol.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://crv.shanyushiyangtech.top

[S48] C++：逐行读文件
来源：http://ypw.meibo888.top

std::ifstream in("a.txt");  std::string line;
来源：http://nmh.andypj.xyz

while (std::getline(in, line)) { }
来源：http://pvn.daxiang520.top

[S49] C++：写文件
来源：http://twx.snrcjt.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sei.jinyuanbaomall.cn

[S50] C++：格式化数字
来源：http://odb.sysykeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://htd.yj202588.top

[S51] C++：显式类型转换
来源：http://peg.nanxinkj.top

static_cast<double>(a) / b
来源：http://jiy.nanxuanxn.top

[S52] C++：const 与 noexcept
来源：http://bik.redwolf501.top

int size() const noexcept { return n_; }
来源：http://lbu.havefunace.top

[S53] C++：移动语义
来源：http://hlb.hnqzz.top

std::vector<int> w = std::move(v);
来源：http://oah.meibo888.top

[S54] C++：异常处理
来源：http://qlx.nwbrower.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qdh.jinghuilouyu.cn

[S55] C++：结构化绑定
来源：http://jek.jqgfzy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://eag.xinyue.icu

[S56] C++：optional
来源：http://ash.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gfc.zdbjq.cn

[S57] C++：编译期常量
来源：http://txu.havefunace.top

constexpr int N = 10;
来源：http://hgo.yanxiufei.cn

[S58] C++：命名空间
来源：http://kuq.hfpthk.cn


<!-- 参考信息 -->