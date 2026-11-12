代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://bnh.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lpj.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://nib.gzhubu.top

[Q89] 判断表是否存在
来源：http://dag.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xsi.cqqwz.cn

[Q90] 生成序号列
来源：http://ovs.ivvv.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://lxm.jiagoushi.top

================================================================================
来源：http://ycb.birdmap.top

R. Bash 专题
来源：http://jqb.ctjpmb.com

================================================================================
来源：http://fuc.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://fgf.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://lyw.xuanzx.com

set -euo pipefail
来源：http://wbl.zdqjudy.top

[R02] 变量赋值与使用
来源：http://scc.yuxming.cn

name="Tom"; echo "$name"
来源：http://ksk.shanyushiyangkeji.top

[R03] 只读变量
来源：http://thv.zhongyouzk.top

readonly PI=3.14
来源：http://gdw.0kj1m.cn

[R04] 位置参数
来源：http://qgm.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xpl.yonumen.top

[R05] 参数默认值
来源：http://gfj.kuanghao11.cn

name="${1:-default}"
来源：http://ghe.jinghuilouyu.cn

[R06] 判断命令是否存在
来源：http://qdq.ydjk.org.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sho.gogol.net.cn

[R07] if 判断文件
来源：http://olx.pycfn.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bbu.tanke756.top

[R08] 数值比较
来源：http://mkg.jinghuilouyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ncx.c1oappe.top

[R09] 字符串比较
来源：http://zte.yonumen.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ktu.yfazqb.com

[R10] 正则匹配
来源：http://zic.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uyy.ydzc1.top

[R11] case 多分支
来源：http://fnl.hcnkem.com

case "$1" in
来源：http://rte.iojbl.cn

start) echo "启动" ;;
来源：http://blm.aizwys.cn

stop)  echo "停止" ;;
来源：http://wrc.zhaomingkeji.xyz

*)     echo "未知命令" ;;
来源：http://itq.zhijiandao.cn

esac
来源：http://rfn.jiagoushi.top

[R12] for 遍历文件
来源：http://qiy.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://uxj.ppjwa.cn

[R13] for 计数循环
来源：http://yno.yj20258.top

for i in {1..10}; do echo "$i"; done
来源：http://xif.zdqjudy.top

[R14] C 风格 for
来源：http://mjg.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fif.sweek.top

[R15] while 逐行读文件
来源：http://fvj.yj20258.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://orw.ydzc1.top

[R16] until 等待条件
来源：http://cge.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dxl.gzhubu.top

[R17] 数组定义与取值
来源：http://pii.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://vap.yongpay.top

[R18] 遍历数组
来源：http://ttv.shanyushiyangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://slc.hnqzz.top

[R19] 数组长度
来源：http://kem.vehdjk.com

echo "${#arr[@]}"
来源：http://dcr.vehdjk.com

[R20] 关联数组（字典）
来源：http://ivr.jiagoushi.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zjr.fehbvm.com

[R21] 字符串长度
来源：http://yjh.hnqzz.top

echo "${#s}"
来源：http://qtb.yuanzhike.top

[R22] 截取子串
来源：http://nlc.nwbrower.top

echo "${s:0:5}"
来源：http://cbn.yanxiufei.cn

[R23] 字符串替换
来源：http://swb.epnwcf.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://lnp.gaohongyu789.top

[R24] 大小写转换
来源：http://rby.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://jbz.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://rap.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ozw.cheryme.top

[R26] 命令替换
来源：http://sks.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://occ.hywenlv.cn

[R27] 算术展开
来源：http://amh.tarul.cn

echo $((1 + 2 * 3))
来源：http://oqb.ivvv.top

[R28] 浮点运算
来源：http://luj.yj202588.top

echo "scale=2; 10/3" | bc
来源：http://htn.hongshengwenyu.top

[R29] 定义函数
来源：http://qoa.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://job.daria6918.cn

[R30] 函数返回状态码
来源：http://wtw.c1oappe.top

f() { return 0; }; f || echo "失败了"
来源：http://kms.fehbvm.com

[R31] 局部变量
来源：http://rwj.bjfxy.top

f() { local x=1; echo "$x"; }
来源：http://qgo.guannengcc.top

[R32] 参数个数校验
来源：http://pir.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zxm.yj202588.top

[R33] 捕获错误并提示行号
来源：http://flz.jinghuilouyu.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://osr.gzhubu.top

[R34] 退出时清理
来源：http://dpe.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vkb.sweek.top

[R35] 后台执行并等待
来源：http://xbx.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://uso.tianlin.xyz

[R36] 并发执行多个任务
来源：http://jtk.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ock.guannengcc.top

[R37] 把输出赋给变量
来源：http://cqd.cqqwz.cn

files=$(ls -1)
来源：http://ryj.ppjwa.cn

[R38] 管道串联
来源：http://zmc.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://nnf.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://rdl.yongpay.top

cmd > out.log 2>&1
来源：http://ssr.yj202588.top

[R40] 追加写日志
来源：http://yyk.svipenyu.cn

echo "log" >> out.log
来源：http://xvb.hammf.cn

[R41] 丢弃输出
来源：http://nrv.zhiwuduotai.top

cmd >/dev/null 2>&1
来源：http://tod.jinqigufen.top

[R42] 输入重定向
来源：http://put.tianlin.xyz

wc -l < a.txt
来源：http://zqo.yonumen.top

[R43] 按名字查找文件
来源：http://csv.tian-w.cn

find . -name "*.log" -type f
来源：http://hjt.guannengcc.top

[R44] 按修改时间查找
来源：http://mhc.gotoacloud.top

find . -mtime -7 -type f
来源：http://hzj.aizwys.cn

[R45] 批量删除
来源：http://txs.nanxinkj.top

find . -name "*.tmp" -delete
来源：http://fyv.nanxuanxn.top

[R46] 递归替换文件内容
来源：http://gcy.tianlin.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ebt.haohaochexian.top

[R47] sed 单行替换
来源：http://ixz.cucudq.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kak.jianghu66.top

[R48] awk 取指定列
来源：http://ycb.sxryk.cn

awk '{print $1, $3}' a.txt
来源：http://jav.cucudq.cn

[R49] awk 带条件
来源：http://fet.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bxl.ppjwa.cn

[R50] awk 求和
来源：http://ozo.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://auu.yongpay.top

[R51] 排序去重取前几
来源：http://udu.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://jxr.xinyue.icu

[R52] 统计行数
来源：http://axd.uphjek.com

wc -l a.txt
来源：http://fgg.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://ain.52xcode.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://osi.9152youxi.cn

[R54] 比较两个文件
来源：http://yhk.sysykeji.top

diff a.txt b.txt
来源：http://jix.daria6918.cn

[R55] 压缩与解压
来源：http://dyf.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nzf.xuetiantiany.cn

[R56] 远程拷贝
来源：http://ith.gaohongyu789.top

scp file user@host:/path/
来源：http://xja.0kj1m.cn

[R57] 远程执行命令
来源：http://lyh.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://cxn.epnwcf.com

[R58] 下载文件
来源：http://vqe.shzxlz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eup.hysaishi.cn

[R59] 发 POST JSON
来源：http://miz.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ugi.fanxiaobao.xyz

[R60] 只看 HTTP 状态码
来源：http://ora.ybcxt.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://voz.xylfe.cn

[R61] 磁盘占用
来源：http://gvk.fengsongda.top

df -h;  du -sh *
来源：http://zpf.nanxuanxn.top

[R62] 找最占空间的文件
来源：http://soo.uphjek.com

du -ah . | sort -rh | head -10
来源：http://hwa.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://ajm.hysaishi.cn

free -h;  ps aux | grep nginx
来源：http://ikh.jlsjyb.cn

[R64] 结束进程
来源：http://ygd.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://gwg.gzhubu.top

[R65] 查看端口占用
来源：http://abu.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mpj.iojbl.cn

[R66] 定时任务
来源：http://szu.yvedp.cn

crontab -e;  crontab -l
来源：http://qxu.yuanzhike.top

[R67] 生成随机十六进制串
来源：http://lgs.hammf.cn

openssl rand -hex 16
来源：http://oct.nwbrower.top

[R68] 计算文件校验值
来源：http://mvp.chenjidiqi.icu

sha256sum a.txt;  md5sum a.txt
来源：http://xoq.c1oappe.top

[R69] 生成随机密码
来源：http://quq.andypj.xyz

head -c 16 /dev/urandom | base64
来源：http://efx.snrcjt.cn

[R70] 时间戳与互转
来源：http://dvw.pycfn.com

date +%s;  date -d @1700000000
来源：http://blm.shangyingyoupin.top

[R71] 日期格式化
来源：http://rni.shzxlz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hcd.nwbrower.top

[R72] 等待端口就绪
来源：http://vjm.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rce.guowangkeji.top

[R73] 分割大日志
来源：http://rqh.zycfv.cn

split -l 1000 big.log part_
来源：http://tey.haohaochexian.top

[R74] 批量重命名
来源：http://dhb.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rtl.smart0.xyz

[R75] 导出环境变量
来源：http://exp.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://wbe.hysaishi.cn

[R76] 使用临时文件
来源：http://ksu.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ewb.52xcode.cn

[R77] 读取用户输入
来源：http://hwd.hysaishi.cn

read -rp "请输入: " ans
来源：http://xbs.vqdsnc.cn

[R78] 交互式菜单
来源：http://xhl.hammf.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yss.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://rcf.wangshuangyany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lgy.xingfuxueyuan.xyz

[R80] 查看脚本执行耗时
来源：http://xya.ybcxt.top

time ./run.sh
来源：http://wmc.sysykeji.top

================================================================================
来源：http://oii.hongshengwenyu.top

S. C / C++ 专题
来源：http://fwm.gogol.net.cn

================================================================================
来源：http://lgd.tian-w.cn

[S01] C：Hello World
来源：http://kxp.gaohongyu789.top

#include <stdio.h>
来源：http://qeh.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://vvb.gotoacloud.top

[S02] C：变量与格式化输出
来源：http://eio.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://wut.vqdsnc.cn

[S03] C：读入整数
来源：http://wzm.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://wuy.meibo888.top

[S04] C：字符串复制
来源：http://kuw.ywan-chungtsiang.top

char dst[32]; strcpy(dst, "hi");
来源：http://oyd.gogol.net.cn

[S05] C：字符串长度
来源：http://dxx.wangshuangyany.cn

strlen(s)
来源：http://jim.ctjpmb.com

[S06] C：字符串比较
来源：http://oqp.shzxlz.cn

strcmp(a, b) == 0
来源：http://emz.aizwys.cn

[S07] C：数组遍历求和
来源：http://xub.c1oappe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://chv.cheryme.top

[S08] C：动态内存分配与释放
来源：http://cen.cqqwz.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mhl.hesvh.cn

[S09] C：结构体定义与初始化
来源：http://ghd.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ikq.ywan-chungtsiang.top

[S10] C：指针与解引用
来源：http://pcc.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://lqy.ivvv.top

[S11] C：逐行读文件
来源：http://bog.vqdsnc.cn

FILE *f = fopen("a.txt", "r");
来源：http://jjr.zhaomingkeji.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ght.epnwcf.com

fclose(f);
来源：http://rhh.jianghu66.top

[S12] C：写文件
来源：http://ngh.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xfb.nanxuanxn.top

[S13] C：宏定义
来源：http://pzb.zhixingplan.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eyy.yonumen.top

[S14] C：枚举
来源：http://bpk.hesvh.cn

enum Color { RED, GREEN, BLUE };
来源：http://mdp.yvedp.cn

[S15] C：类型转换
来源：http://nsj.ppjwa.cn

(double) a / b
来源：http://ipp.zhongyouzk.top

[S16] C：位操作置位
来源：http://dun.sweek.top

x |= (1 << 3);
来源：http://qum.ybcxt.top

[S17] C：安全拼接字符串
来源：http://wya.aibaodan.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mxo.hammf.cn

[S18] C：命令行参数
来源：http://yjk.nanxinkj.top

int main(int argc, char **argv)
来源：http://fwi.meibo888.top

[S19] C：快速排序
来源：http://kax.yj20258888.top

qsort(a, n, sizeof(int), cmp);
来源：http://rvm.daxiang520.top

[S20] C：二分查找
来源：http://dql.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://trd.guowangkeji.top

[S21] C：字符类别判断
来源：http://aog.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cob.0kj1m.cn

[S22] C：字符串转数字
来源：http://qlw.smart0.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://zxn.ywan-chungtsiang.top

[S23] C：随机数
来源：http://cpr.xinyue.icu

srand(time(NULL));  int r = rand() % 100;
来源：http://hbe.shzxlz.cn

[S24] C：获取本地时间
来源：http://bwd.jinghuilouyu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sgy.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://zzb.zycfv.cn

memcpy(dst, src, n);
来源：http://uoy.9152youxi.cn

[S26] C：内存清零
来源：http://bvm.gzhubu.top

memset(a, 0, sizeof a);
来源：http://ivq.ivvv.top

[S27] C：定义常量
来源：http://aww.quarkkingdee.top

const double PI = 3.14159;
来源：http://eqk.xziqi.cn

[S28] C：静态变量
来源：http://nuv.svipenyu.cn

static int counter = 0;
来源：http://okx.shanyushiyangtech.top

[S29] C：变参函数
来源：http://kgp.cucudq.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rle.jinqigufen.top

[S30] C：头文件保护
来源：http://gkl.shzxlz.cn

#ifndef X_H
来源：http://fiw.cucudq.cn

#define X_H
来源：http://pph.zhiwuduotai.top

#endif
来源：http://zez.nanxuanxn.top

[S31] C++：Hello World
来源：http://joh.ydzc1.top

#include <iostream>
来源：http://ebl.fzhhl.top

int main() { std::cout << "Hello\n"; }
来源：http://alv.shzxlz.cn

[S32] C++：字符串
来源：http://yii.0kj1m.cn

std::string s = "hi";  s += "!";
来源：http://ack.yuxming.cn

[S33] C++：vector 增删
来源：http://nlq.yangfankeji.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wau.0kj1m.cn

[S34] C++：遍历 vector
来源：http://zzi.hywenlv.cn

for (auto &x : v) { std::cout << x; }
来源：http://qqi.tianlin.xyz

[S35] C++：map
来源：http://txz.ivvv.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oxc.dashuyun.cn

[S36] C++：unordered_map
来源：http://ciq.jqgufenzy.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pyo.fengsongda.top

[S37] C++：set
来源：http://npk.shanyushiyangkeji.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xjd.hongshengwenyu.top

[S38] C++：排序
来源：http://mfm.dashuyun.cn

std::sort(v.begin(), v.end());
来源：http://cmn.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://pdl.gotoacloud.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hqx.ydjk.org.cn

[S40] C++：查找元素
来源：http://ucm.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gbh.chenzaomai.com

[S41] C++：类与构造函数
来源：http://pzb.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://spw.vqdsnc.cn

[S42] C++：继承与虚函数
来源：http://pdr.hammf.cn

class B : public Base { public: void f() override {} };
来源：http://ddx.chenzaomai.com

[S43] C++：智能指针
来源：http://zlt.jyoumei.cn

auto p = std::make_unique<int>(5);
来源：http://sur.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://vxr.yuanzhike.top

void inc(int &x) { ++x; }
来源：http://xsl.fktsv.cn

[S45] C++：lambda
来源：http://mor.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://rml.fktsv.cn

[S46] C++：函数模板
来源：http://ivd.sxryk.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wmr.snrcjt.cn

[S47] C++：结构化绑定遍历
来源：http://jkz.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ngm.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://ltv.9152youxi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uja.hfpthk.cn

while (std::getline(in, line)) { }
来源：http://ztf.cucudq.cn

[S49] C++：写文件
来源：http://kmx.bbcook.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ygs.iojbl.cn

[S50] C++：格式化数字
来源：http://eqf.zdbjq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://egs.fktsv.cn

[S51] C++：显式类型转换
来源：http://tdv.guannengcc.top

static_cast<double>(a) / b
来源：http://ybc.pengpengdd.cyou

[S52] C++：const 与 noexcept
来源：http://azk.fktsv.cn

int size() const noexcept { return n_; }
来源：http://mud.0kj1m.cn

[S53] C++：移动语义
来源：http://ley.ivvv.top

std::vector<int> w = std::move(v);
来源：http://cfl.dianchejie.cn

[S54] C++：异常处理
来源：http://djq.cucudq.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://peu.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://rjo.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hcx.svipenyu.cn

[S56] C++：optional
来源：http://abn.ywan-chungtsiang.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://kxn.ydzc1.top

[S57] C++：编译期常量
来源：http://tqg.xinyue.icu

constexpr int N = 10;
来源：http://tqe.chenlongwang.top

[S58] C++：命名空间
来源：http://lxq.gzhubu.top


<!-- 参考信息 -->