代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vkq.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://wyi.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bkc.jqgufenzy.top

================================================================================
来源：http://npr.jyoumei.cn

R. Bash 专题
来源：http://uuk.bbcook.cn

================================================================================
来源：http://owp.xuanzx.com

[R01] shebang 与严格模式
来源：http://auc.zhoulong.xyz

#!/usr/bin/env bash
来源：http://yrn.ppjwa.cn

set -euo pipefail
来源：http://ilj.feifeiyinyue.top

[R02] 变量赋值与使用
来源：http://tlf.smart0.xyz

name="Tom"; echo "$name"
来源：http://fnt.quarkkingdee.top

[R03] 只读变量
来源：http://aaz.tian-w.cn

readonly PI=3.14
来源：http://mjn.iojbl.cn

[R04] 位置参数
来源：http://wdi.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jyy.zhiwuduotai.top

[R05] 参数默认值
来源：http://wui.tian-w.cn

name="${1:-default}"
来源：http://aoa.cqqwz.cn

[R06] 判断命令是否存在
来源：http://qto.gogol.net.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://paq.wangdashe.top

[R07] if 判断文件
来源：http://gdv.redwolf501.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zmr.bbcook.cn

[R08] 数值比较
来源：http://jfx.gaohongyu789.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zoq.svipenyu.cn

[R09] 字符串比较
来源：http://qgy.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fjb.birdmap.top

[R10] 正则匹配
来源：http://qby.c1oappe.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://euc.haohaochexian.top

[R11] case 多分支
来源：http://inf.uphjek.com

case "$1" in
来源：http://ddg.hywenlv.cn

start) echo "启动" ;;
来源：http://mos.sysykeji.top

stop)  echo "停止" ;;
来源：http://qrk.wangdashe.top

*)     echo "未知命令" ;;
来源：http://cuo.shuidangran.top

esac
来源：http://jfj.smart0.xyz

[R12] for 遍历文件
来源：http://pad.c1oappe.top

for f in *.txt; do echo "$f"; done
来源：http://skf.yfazqb.com

[R13] for 计数循环
来源：http://enn.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://hpr.ppjwa.cn

[R14] C 风格 for
来源：http://crp.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kcj.nanxuanxn.top

[R15] while 逐行读文件
来源：http://tnu.wangshuangyany.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mwf.tanke756.top

[R16] until 等待条件
来源：http://fsj.9152youxi.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xtc.cdnleiting.top

[R17] 数组定义与取值
来源：http://ejg.ppjwa.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zgy.sufxvd.cn

[R18] 遍历数组
来源：http://fyo.bbcook.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uxt.ybcxt.top

[R19] 数组长度
来源：http://gtz.epnwcf.com

echo "${#arr[@]}"
来源：http://bit.cheryme.top

[R20] 关联数组（字典）
来源：http://uzm.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xye.cqqwz.cn

[R21] 字符串长度
来源：http://rnq.cashguo.top

echo "${#s}"
来源：http://mez.tianlin.xyz

[R22] 截取子串
来源：http://fal.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://afd.shanyushiyangtech.top

[R23] 字符串替换
来源：http://aun.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cve.andypj.xyz

[R24] 大小写转换
来源：http://feg.daxiang520.top

echo "${s^^}"; echo "${s,,}"
来源：http://aaa.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://ywk.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://msz.hysaishi.cn

[R26] 命令替换
来源：http://gbb.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://hsj.hesvh.cn

[R27] 算术展开
来源：http://gmw.zhaomingkeji.xyz

echo $((1 + 2 * 3))
来源：http://kii.yuanzhike.top

[R28] 浮点运算
来源：http://jim.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://wup.jinqigufen.top

[R29] 定义函数
来源：http://sqx.yj202588.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ava.zhengqikj.top

[R30] 函数返回状态码
来源：http://gqd.xingfuxueyuan.xyz

f() { return 0; }; f || echo "失败了"
来源：http://ven.yj20258888.top

[R31] 局部变量
来源：http://ahj.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://qhg.jianghu66.top

[R32] 参数个数校验
来源：http://zun.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://msn.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://obv.zhoulong.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ngi.ywan-chungtsiang.top

[R34] 退出时清理
来源：http://aqp.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://yvy.guannengcc.top

[R35] 后台执行并等待
来源：http://ild.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://aug.svipenyu.cn

[R36] 并发执行多个任务
来源：http://ywd.fanxiaobao.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hws.fengsongda.top

[R37] 把输出赋给变量
来源：http://khl.bjfxy.top

files=$(ls -1)
来源：http://pww.pycfn.com

[R38] 管道串联
来源：http://fug.jiagoushi.top

cat a.txt | grep -i error | wc -l
来源：http://ucs.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://qwo.bbcook.cn

cmd > out.log 2>&1
来源：http://lro.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://grn.yongpay.top

echo "log" >> out.log
来源：http://itj.jyoumei.cn

[R41] 丢弃输出
来源：http://rsm.zhixingplan.top

cmd >/dev/null 2>&1
来源：http://bgf.jqgfzy.top

[R42] 输入重定向
来源：http://tbe.xuetiantiany.cn

wc -l < a.txt
来源：http://vxx.gogol.net.cn

[R43] 按名字查找文件
来源：http://owa.fzhhl.top

find . -name "*.log" -type f
来源：http://tog.fengsongda.top

[R44] 按修改时间查找
来源：http://zzg.hcnkem.com

find . -mtime -7 -type f
来源：http://sni.yongpay.top

[R45] 批量删除
来源：http://oyy.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://fnu.cheryme.top

[R46] 递归替换文件内容
来源：http://zln.fzhhl.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pyw.guowangkeji.top

[R47] sed 单行替换
来源：http://tpv.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://wtq.dianchejie.cn

[R48] awk 取指定列
来源：http://vaw.wangshuangyany.cn

awk '{print $1, $3}' a.txt
来源：http://hzm.zhongyouzk.top

[R49] awk 带条件
来源：http://xct.jinyuanbaomall.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bsd.ywan-chungtsiang.top

[R50] awk 求和
来源：http://glt.wangdashe.top

awk '{s += $2} END {print s}' a.txt
来源：http://rml.yj202588.top

[R51] 排序去重取前几
来源：http://iqs.shuidangran.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ecd.cashguo.top

[R52] 统计行数
来源：http://pme.jinyuanbaomall.cn

wc -l a.txt
来源：http://tsd.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://zxm.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tlz.epnwcf.com

[R54] 比较两个文件
来源：http://gnx.hongshengwenyu.top

diff a.txt b.txt
来源：http://txp.hcnkem.com

[R55] 压缩与解压
来源：http://yyq.zdqjudy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://neu.hammf.cn

[R56] 远程拷贝
来源：http://dqf.zdqjudy.top

scp file user@host:/path/
来源：http://frn.shangyingyoupin.top

[R57] 远程执行命令
来源：http://jkn.shangyingyoupin.top

ssh user@host 'uptime'
来源：http://oga.andypj.xyz

[R58] 下载文件
来源：http://jfn.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://awl.hnxiangtu.top

[R59] 发 POST JSON
来源：http://iwc.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eew.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://nsz.andypj.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nyx.chenjidiqi.icu

[R61] 磁盘占用
来源：http://gco.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://bet.cashguo.top

[R62] 找最占空间的文件
来源：http://ehm.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://nfp.yongpay.top

[R63] 内存与进程
来源：http://xmi.316326.xyz

free -h;  ps aux | grep nginx
来源：http://xyf.quarkkingdee.top

[R64] 结束进程
来源：http://wgz.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://sdn.smart0.xyz

[R65] 查看端口占用
来源：http://zef.wangdashe.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gxp.jiagoushi.top

[R66] 定时任务
来源：http://yvz.jinqigufen.top

crontab -e;  crontab -l
来源：http://vvn.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://xew.jinyuanbaomall.cn

openssl rand -hex 16
来源：http://pxn.smart0.xyz

[R68] 计算文件校验值
来源：http://gnp.jinghuilouyu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ehz.meibo888.top

[R69] 生成随机密码
来源：http://ljh.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://dnv.dianchejie.cn

[R70] 时间戳与互转
来源：http://dbs.daria6918.cn

date +%s;  date -d @1700000000
来源：http://ryw.shuidangran.top

[R71] 日期格式化
来源：http://aap.cheryme.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://cvd.yongpay.top

[R72] 等待端口就绪
来源：http://hie.shanyushiyangkeji.top

until nc -z localhost 3306; do sleep 1; done
来源：http://foo.jqgfzy.top

[R73] 分割大日志
来源：http://teb.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://qgl.kuanghao11.cn

[R74] 批量重命名
来源：http://pbh.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tay.jqgufenzy.top

[R75] 导出环境变量
来源：http://tfo.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://qrd.epnwcf.com

[R76] 使用临时文件
来源：http://mfh.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://min.shuidangran.top

[R77] 读取用户输入
来源：http://dvp.uphjek.com

read -rp "请输入: " ans
来源：http://fnk.yanxiufei.cn

[R78] 交互式菜单
来源：http://xzp.zhiwuduotai.top

select opt in a b c; do echo "$opt"; break; done
来源：http://sye.epnwcf.com

[R79] 解析命令行选项
来源：http://jll.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nus.cdnleiting.top

[R80] 查看脚本执行耗时
来源：http://ysw.sweek.top

time ./run.sh
来源：http://ftl.andypj.xyz

================================================================================
来源：http://zlo.wangdashe.top

S. C / C++ 专题
来源：http://gjs.jqgfzy.top

================================================================================
来源：http://gaj.tian-w.cn

[S01] C：Hello World
来源：http://ymk.shangyingyoupin.top

#include <stdio.h>
来源：http://xrr.uphjek.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://lxi.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://wrp.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://qdq.yuxming.cn

[S03] C：读入整数
来源：http://vtm.xziqi.cn

int x; scanf("%d", &x);
来源：http://rtx.zycfv.cn

[S04] C：字符串复制
来源：http://zhw.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://wig.yangfankeji.com

[S05] C：字符串长度
来源：http://twv.snrcjt.cn

strlen(s)
来源：http://dza.0kj1m.cn

[S06] C：字符串比较
来源：http://mde.zycfv.cn

strcmp(a, b) == 0
来源：http://bfu.daria6918.cn

[S07] C：数组遍历求和
来源：http://ulm.guowangkeji.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pnp.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://esf.iojbl.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://amz.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://ooa.fengsongda.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wyi.shangyingyoupin.top

[S10] C：指针与解引用
来源：http://bbl.sweek.top

int *p = &a;  *p = 5;
来源：http://eus.xuanzx.com

[S11] C：逐行读文件
来源：http://rjs.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://iig.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://xlu.daxiang520.top

fclose(f);
来源：http://tey.cdnleiting.top

[S12] C：写文件
来源：http://lpe.svipenyu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ixi.fktsv.cn

[S13] C：宏定义
来源：http://ohw.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kbq.ywan-chungtsiang.top

[S14] C：枚举
来源：http://bvx.shangyingyoupin.top

enum Color { RED, GREEN, BLUE };
来源：http://fiv.yvedp.cn

[S15] C：类型转换
来源：http://yit.yongpay.top

(double) a / b
来源：http://xiu.sufxvd.cn

[S16] C：位操作置位
来源：http://mra.sxryk.cn

x |= (1 << 3);
来源：http://qkh.xinyue.icu

[S17] C：安全拼接字符串
来源：http://spx.zhiwuduotai.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gho.yj20258.top

[S18] C：命令行参数
来源：http://qji.guannengcc.top

int main(int argc, char **argv)
来源：http://nnn.yj20258.top

[S19] C：快速排序
来源：http://muk.tarul.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uby.xziqi.cn

[S20] C：二分查找
来源：http://uxj.yongpay.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://efw.bjfxy.top

[S21] C：字符类别判断
来源：http://mux.0kj1m.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rnz.ehwqpu.com

[S22] C：字符串转数字
来源：http://jef.ppjwa.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zpg.gotoacloud.top

[S23] C：随机数
来源：http://vxo.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://doe.wangdashe.top

[S24] C：获取本地时间
来源：http://zwh.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zii.xziqi.cn

[S25] C：内存拷贝
来源：http://gse.zdbjq.cn

memcpy(dst, src, n);
来源：http://arp.iojbl.cn

[S26] C：内存清零
来源：http://jls.yueranfly.top

memset(a, 0, sizeof a);
来源：http://qqb.svipenyu.cn

[S27] C：定义常量
来源：http://gvl.hongshengwenyu.top

const double PI = 3.14159;
来源：http://dtm.hcnkem.com

[S28] C：静态变量
来源：http://sgx.feifeiyinyue.top

static int counter = 0;
来源：http://efz.wangdashe.top

[S29] C：变参函数
来源：http://ldy.zhiwuduotai.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uiz.nwbrower.top

[S30] C：头文件保护
来源：http://sew.jyoumei.cn

#ifndef X_H
来源：http://wmo.sufxvd.cn

#define X_H
来源：http://qlm.vehdjk.com

#endif
来源：http://oao.zhengqikj.top

[S31] C++：Hello World
来源：http://amq.daxiang520.top

#include <iostream>
来源：http://vpo.hnxiangtu.top

int main() { std::cout << "Hello\n"; }
来源：http://czu.shzxlz.cn

[S32] C++：字符串
来源：http://pcc.zhongyouzk.top

std::string s = "hi";  s += "!";
来源：http://pms.yueranfly.top

[S33] C++：vector 增删
来源：http://fov.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wcf.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://fyn.fzhhl.top

for (auto &x : v) { std::cout << x; }
来源：http://cgs.jyoumei.cn

[S35] C++：map
来源：http://wbj.shanyushiyangkeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bsp.dianchejie.cn

[S36] C++：unordered_map
来源：http://yyw.bjfxy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fgh.hysaishi.cn

[S37] C++：set
来源：http://dds.zhoulong.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pyf.shzxlz.cn

[S38] C++：排序
来源：http://vdm.xingfuxueyuan.xyz

std::sort(v.begin(), v.end());
来源：http://oxl.9152youxi.cn

[S39] C++：自定义比较器排序
来源：http://vca.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://okm.guannengcc.top

[S40] C++：查找元素
来源：http://xum.bbcook.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xea.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://htk.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zta.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://sbp.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://oun.yuanzhike.top

[S43] C++：智能指针
来源：http://ngy.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://lax.zycfv.cn

[S44] C++：引用传参
来源：http://dsk.yj202588.top

void inc(int &x) { ++x; }
来源：http://jtx.aizwys.cn

[S45] C++：lambda
来源：http://njl.52xcode.cn

auto add = [](int a, int b) { return a + b; };
来源：http://mko.zhengqikj.top

[S46] C++：函数模板
来源：http://sdy.zhaomingkeji.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://esm.yongpay.top

[S47] C++：结构化绑定遍历
来源：http://zuv.daria6918.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xmn.gzhubu.top

[S48] C++：逐行读文件
来源：http://tle.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dvo.yuxming.cn

while (std::getline(in, line)) { }
来源：http://fdv.cheryme.top

[S49] C++：写文件
来源：http://kad.jiagoushi.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ngm.redwolf501.top

[S50] C++：格式化数字
来源：http://mop.mhx1999.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ofr.wangshuangyany.cn

[S51] C++：显式类型转换
来源：http://gec.jqgfzy.top

static_cast<double>(a) / b
来源：http://oqz.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://jce.gotoacloud.top

int size() const noexcept { return n_; }
来源：http://dhl.ppjwa.cn

[S53] C++：移动语义
来源：http://eeh.yfazqb.com

std::vector<int> w = std::move(v);
来源：http://ivh.gogol.net.cn

[S54] C++：异常处理
来源：http://tbt.pycfn.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://etm.hnqzz.top

[S55] C++：结构化绑定
来源：http://pat.shzxlz.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iai.gotoacloud.top

[S56] C++：optional
来源：http://jfs.pengpengdd.cyou

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fxa.snrcjt.cn

[S57] C++：编译期常量
来源：http://kbj.guannengcc.top

constexpr int N = 10;
来源：http://tak.ybcxt.top

[S58] C++：命名空间
来源：http://tjf.sjlbkw.cn

namespace ns { int f() { return 1; } }
来源：http://klg.shuidangran.top

[S59] C++：静态断言
来源：http://zwn.cheryme.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cyr.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://jgc.gotoacloud.top


<!-- 参考信息 -->