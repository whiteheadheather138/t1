代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dju.xylfe.cn

[Q90] 生成序号列
来源：http://cje.zhaomingkeji.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ath.hcnkem.com

================================================================================
来源：http://elc.jinyuanbaomall.cn

R. Bash 专题
来源：http://njk.bjfxy.top

================================================================================
来源：http://ddo.aizwys.cn

[R01] shebang 与严格模式
来源：http://pjg.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://rdd.tanke756.top

set -euo pipefail
来源：http://ykr.jinghuilouyu.cn

[R02] 变量赋值与使用
来源：http://jxj.pycfn.com

name="Tom"; echo "$name"
来源：http://jzt.zycfv.cn

[R03] 只读变量
来源：http://hxz.hfpthk.cn

readonly PI=3.14
来源：http://fnc.cdnleiting.top

[R04] 位置参数
来源：http://qme.bjfxy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://rfq.zhoulong.xyz

[R05] 参数默认值
来源：http://vdf.tarul.cn

name="${1:-default}"
来源：http://qiw.aibaodan.cn

[R06] 判断命令是否存在
来源：http://srn.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wbc.birdmap.top

[R07] if 判断文件
来源：http://uok.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hht.dashuyun.cn

[R08] 数值比较
来源：http://amu.bjfxy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ife.chenlongwang.top

[R09] 字符串比较
来源：http://hgv.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dvi.hesvh.cn

[R10] 正则匹配
来源：http://oqa.hfpthk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qwc.smart0.xyz

[R11] case 多分支
来源：http://icv.bbcook.cn

case "$1" in
来源：http://vgg.wangdashe.top

start) echo "启动" ;;
来源：http://lyi.bjfxy.top

stop)  echo "停止" ;;
来源：http://jvj.bbcook.cn

*)     echo "未知命令" ;;
来源：http://yoi.shuidangran.top

esac
来源：http://nay.shzxlz.cn

[R12] for 遍历文件
来源：http://xck.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://grx.zhongyouzk.top

[R13] for 计数循环
来源：http://yzf.zhijiandao.cn

for i in {1..10}; do echo "$i"; done
来源：http://gef.yj20258.top

[R14] C 风格 for
来源：http://kwv.kuanghao11.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lki.jinghuilouyu.cn

[R15] while 逐行读文件
来源：http://jyf.xuetiantiany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://enq.9152youxi.cn

[R16] until 等待条件
来源：http://bev.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hux.yvedp.cn

[R17] 数组定义与取值
来源：http://olp.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://bts.uphjek.com

[R18] 遍历数组
来源：http://imv.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kbm.yj20258.top

[R19] 数组长度
来源：http://cxk.dashuyun.cn

echo "${#arr[@]}"
来源：http://skt.xinyue.icu

[R20] 关联数组（字典）
来源：http://fza.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jnw.zhoulong.xyz

[R21] 字符串长度
来源：http://plk.yuanzhike.top

echo "${#s}"
来源：http://zcu.shanyushiyangkeji.top

[R22] 截取子串
来源：http://gaf.xylfe.cn

echo "${s:0:5}"
来源：http://zyr.shuidangran.top

[R23] 字符串替换
来源：http://htb.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hka.yuanzhike.top

[R24] 大小写转换
来源：http://fkw.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://wke.sjlbkw.cn

[R25] 去后缀 / 去前缀
来源：http://umj.ivvv.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vrz.daxiang520.top

[R26] 命令替换
来源：http://xru.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://lxn.zdqjudy.top

[R27] 算术展开
来源：http://rbk.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://qwu.yj20258.top

[R28] 浮点运算
来源：http://vok.havefunace.top

echo "scale=2; 10/3" | bc
来源：http://wvb.tian-w.cn

[R29] 定义函数
来源：http://mln.xuanzx.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kkj.aibaodan.cn

[R30] 函数返回状态码
来源：http://zee.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://jwl.yonumen.top

[R31] 局部变量
来源：http://zrx.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://huq.yj202588.top

[R32] 参数个数校验
来源：http://qjm.dashuyun.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mrh.zhongyouzk.top

[R33] 捕获错误并提示行号
来源：http://itb.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jzq.hywenlv.cn

[R34] 退出时清理
来源：http://wup.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jcj.hcnkem.com

[R35] 后台执行并等待
来源：http://fwr.guowangkeji.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yfz.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://yao.yongpay.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tlk.daxiang520.top

[R37] 把输出赋给变量
来源：http://tlm.feifeiyinyue.top

files=$(ls -1)
来源：http://wnk.kuanghao11.cn

[R38] 管道串联
来源：http://cyd.aizwys.cn

cat a.txt | grep -i error | wc -l
来源：http://goj.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://yks.zhixingplan.top

cmd > out.log 2>&1
来源：http://qcw.jianghu66.top

[R40] 追加写日志
来源：http://qha.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://jkv.cqqwz.cn

[R41] 丢弃输出
来源：http://lsu.dianchejie.cn

cmd >/dev/null 2>&1
来源：http://yto.zhiwuduotai.top

[R42] 输入重定向
来源：http://fmj.jyoumei.cn

wc -l < a.txt
来源：http://ivo.tanke756.top

[R43] 按名字查找文件
来源：http://pox.sysykeji.top

find . -name "*.log" -type f
来源：http://rif.zhengqikj.top

[R44] 按修改时间查找
来源：http://rho.dashuyun.cn

find . -mtime -7 -type f
来源：http://rcp.fengsongda.top

[R45] 批量删除
来源：http://ont.zdbjq.cn

find . -name "*.tmp" -delete
来源：http://puy.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://vng.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sbj.vqdsnc.cn

[R47] sed 单行替换
来源：http://gpv.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://buq.hammf.cn

[R48] awk 取指定列
来源：http://rmu.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://fxz.jqgfzy.top

[R49] awk 带条件
来源：http://awc.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yke.vqdsnc.cn

[R50] awk 求和
来源：http://eoc.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://bga.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://quf.gotoacloud.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sfo.fktsv.cn

[R52] 统计行数
来源：http://njz.hesvh.cn

wc -l a.txt
来源：http://pag.sufxvd.cn

[R53] 查看文件头与实时尾
来源：http://gfx.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hxv.ybcxt.top

[R54] 比较两个文件
来源：http://xgt.shanyushiyangkeji.top

diff a.txt b.txt
来源：http://guk.redwolf501.top

[R55] 压缩与解压
来源：http://rzu.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uri.feifeiyinyue.top

[R56] 远程拷贝
来源：http://vch.redwolf501.top

scp file user@host:/path/
来源：http://twd.aibaodan.cn

[R57] 远程执行命令
来源：http://acd.jinyuanbaomall.cn

ssh user@host 'uptime'
来源：http://qkf.52xcode.cn

[R58] 下载文件
来源：http://eih.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://twu.c1oappe.top

[R59] 发 POST JSON
来源：http://npr.guannengcc.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zpq.cdnleiting.top

[R60] 只看 HTTP 状态码
来源：http://pdw.ehwqpu.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://eru.jyoumei.cn

[R61] 磁盘占用
来源：http://iga.316326.xyz

df -h;  du -sh *
来源：http://afv.sxryk.cn

[R62] 找最占空间的文件
来源：http://fqw.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://akj.yfazqb.com

[R63] 内存与进程
来源：http://agp.jyoumei.cn

free -h;  ps aux | grep nginx
来源：http://qdf.snrcjt.cn

[R64] 结束进程
来源：http://cuz.svipenyu.cn

kill -9 $(pgrep -f app.py)
来源：http://fyr.birdmap.top

[R65] 查看端口占用
来源：http://tce.zhixingplan.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fwq.hnxiangtu.top

[R66] 定时任务
来源：http://fhb.jiagoushi.top

crontab -e;  crontab -l
来源：http://eww.sxryk.cn

[R67] 生成随机十六进制串
来源：http://pof.vqdsnc.cn

openssl rand -hex 16
来源：http://apz.yj20258888.top

[R68] 计算文件校验值
来源：http://zaq.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://okx.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://nbr.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://pwm.zhoulong.xyz

[R70] 时间戳与互转
来源：http://gok.daria6918.cn

date +%s;  date -d @1700000000
来源：http://hvc.yongpay.top

[R71] 日期格式化
来源：http://fjs.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://hes.zhijiandao.cn

[R72] 等待端口就绪
来源：http://fin.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://evb.c1oappe.top

[R73] 分割大日志
来源：http://wwc.guannengcc.top

split -l 1000 big.log part_
来源：http://vjk.hfpthk.cn

[R74] 批量重命名
来源：http://njl.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ysg.sjlbkw.cn

[R75] 导出环境变量
来源：http://mrg.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://fku.dashuyun.cn

[R76] 使用临时文件
来源：http://rwj.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://iwa.c1oappe.top

[R77] 读取用户输入
来源：http://olu.dianchejie.cn

read -rp "请输入: " ans
来源：http://oqn.yj20258888.top

[R78] 交互式菜单
来源：http://hrz.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wgb.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://uij.ywan-chungtsiang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qlx.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://swq.xuanzx.com

time ./run.sh
来源：http://skc.cqqwz.cn

================================================================================
来源：http://ody.xylfe.cn

S. C / C++ 专题
来源：http://wgz.zhixingplan.top

================================================================================
来源：http://utv.yfazqb.com

[S01] C：Hello World
来源：http://osj.snrcjt.cn

#include <stdio.h>
来源：http://tat.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://tul.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://aza.tarul.cn

int a = 10; printf("%d\n", a);
来源：http://qge.vqdsnc.cn

[S03] C：读入整数
来源：http://osf.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://bxs.sufxvd.cn

[S04] C：字符串复制
来源：http://enw.zdqjudy.top

char dst[32]; strcpy(dst, "hi");
来源：http://lyl.zhixingplan.top

[S05] C：字符串长度
来源：http://vqu.pycfn.com

strlen(s)
来源：http://usp.svipenyu.cn

[S06] C：字符串比较
来源：http://msa.chenjidiqi.icu

strcmp(a, b) == 0
来源：http://pbg.jinqigufen.top

[S07] C：数组遍历求和
来源：http://tkg.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gil.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://giu.shzxlz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oqq.shzxlz.cn

[S09] C：结构体定义与初始化
来源：http://kgk.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iha.chenlongwang.top

[S10] C：指针与解引用
来源：http://kyw.jiagoushi.top

int *p = &a;  *p = 5;
来源：http://jqw.zhengqikj.top

[S11] C：逐行读文件
来源：http://apw.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://lju.shangyingyoupin.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kwv.nwbrower.top

fclose(f);
来源：http://jar.yueranfly.top

[S12] C：写文件
来源：http://mhg.epnwcf.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fzg.xuetiantiany.cn

[S13] C：宏定义
来源：http://yrb.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pgx.chenzaomai.com

[S14] C：枚举
来源：http://unc.ydzc1.top

enum Color { RED, GREEN, BLUE };
来源：http://oho.zhijiandao.cn

[S15] C：类型转换
来源：http://ixs.aizwys.cn

(double) a / b
来源：http://wdb.gaohongyu789.top

[S16] C：位操作置位
来源：http://vvx.yvedp.cn

x |= (1 << 3);
来源：http://efr.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://cpr.daria6918.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nzf.feifeiyinyue.top

[S18] C：命令行参数
来源：http://rlr.sjlbkw.cn

int main(int argc, char **argv)
来源：http://mcr.guowangkeji.top

[S19] C：快速排序
来源：http://lap.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vkp.yangfankeji.com

[S20] C：二分查找
来源：http://lpg.sjlbkw.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rgj.nanxuanxn.top

[S21] C：字符类别判断
来源：http://xtv.9152youxi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://evl.xziqi.cn

[S22] C：字符串转数字
来源：http://qno.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://jck.shanyushiyangkeji.top

[S23] C：随机数
来源：http://nio.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://npq.fengsongda.top

[S24] C：获取本地时间
来源：http://hon.iojbl.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fqv.fzhhl.top

[S25] C：内存拷贝
来源：http://sqi.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://akd.zdbjq.cn

[S26] C：内存清零
来源：http://gmo.yfazqb.com

memset(a, 0, sizeof a);
来源：http://fdr.cashguo.top

[S27] C：定义常量
来源：http://qmr.aibaodan.cn

const double PI = 3.14159;
来源：http://blx.yonumen.top

[S28] C：静态变量
来源：http://xoj.cdnleiting.top

static int counter = 0;
来源：http://qpx.guannengcc.top

[S29] C：变参函数
来源：http://awv.fanxiaobao.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gug.cashguo.top

[S30] C：头文件保护
来源：http://vvr.jqgfzy.top

#ifndef X_H
来源：http://mda.mhx1999.top

#define X_H
来源：http://cld.xziqi.cn

#endif
来源：http://xcg.yonumen.top

[S31] C++：Hello World
来源：http://tpq.jqgfzy.top

#include <iostream>
来源：http://igd.nanxuanxn.top

int main() { std::cout << "Hello\n"; }
来源：http://sth.tian-w.cn

[S32] C++：字符串
来源：http://djn.daxiang520.top

std::string s = "hi";  s += "!";
来源：http://iga.yongpay.top

[S33] C++：vector 增删
来源：http://mjv.cdnleiting.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ery.dianchejie.cn

[S34] C++：遍历 vector
来源：http://brw.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://esd.andypj.xyz

[S35] C++：map
来源：http://ydv.fanxiaobao.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lsb.zdqjudy.top

[S36] C++：unordered_map
来源：http://bhj.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uww.sufxvd.cn

[S37] C++：set
来源：http://cif.zhiwuduotai.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ozp.sxryk.cn

[S38] C++：排序
来源：http://gzz.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://oqv.ehwqpu.com

[S39] C++：自定义比较器排序
来源：http://ekv.jinqigufen.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aep.vehdjk.com

[S40] C++：查找元素
来源：http://ehg.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zux.mhx1999.top

[S41] C++：类与构造函数
来源：http://tij.jinqigfzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wwk.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://emu.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://fqf.ctjpmb.com

[S43] C++：智能指针
来源：http://qjj.shanyushiyangkeji.top

auto p = std::make_unique<int>(5);
来源：http://evz.zhiwuduotai.top

[S44] C++：引用传参
来源：http://uqt.yangfankeji.com

void inc(int &x) { ++x; }
来源：http://nue.fehbvm.com

[S45] C++：lambda
来源：http://ued.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://dau.yanxiufei.cn

[S46] C++：函数模板
来源：http://nkv.jinyuanbaomall.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nle.yfazqb.com

[S47] C++：结构化绑定遍历
来源：http://wcx.9152youxi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ktz.yj20258.top

[S48] C++：逐行读文件
来源：http://yli.zhengqikj.top

std::ifstream in("a.txt");  std::string line;
来源：http://xds.chenjidiqi.icu

while (std::getline(in, line)) { }
来源：http://mto.yanxiufei.cn

[S49] C++：写文件
来源：http://msm.hnxiangtu.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ilm.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://cic.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lol.dianchejie.cn

[S51] C++：显式类型转换
来源：http://ios.feifeiyinyue.top

static_cast<double>(a) / b
来源：http://wsg.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://kaj.fzhhl.top

int size() const noexcept { return n_; }
来源：http://wmy.yuxming.cn

[S53] C++：移动语义
来源：http://qpn.shangyingyoupin.top

std::vector<int> w = std::move(v);
来源：http://njc.daria6918.cn

[S54] C++：异常处理
来源：http://yne.hnqzz.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nmb.shzxlz.cn

[S55] C++：结构化绑定
来源：http://ofd.quarkkingdee.top

auto [a, b] = std::make_pair(1, 2);
来源：http://yik.shzxlz.cn

[S56] C++：optional
来源：http://jax.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://skk.fanxiaobao.xyz

[S57] C++：编译期常量
来源：http://iju.hongshengwenyu.top

constexpr int N = 10;
来源：http://vvm.aizwys.cn

[S58] C++：命名空间
来源：http://hwp.hnxiangtu.top

namespace ns { int f() { return 1; } }
来源：http://wwa.quarkkingdee.top

[S59] C++：静态断言
来源：http://inw.epnwcf.com

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://lby.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://omw.ydzc1.top


<!-- 参考信息 -->