代发 wailian999

[Q84] 去除首尾空格
来源：http://frx.wangshuangyany.cn

SELECT TRIM(name) FROM users;
来源：http://vzo.dashuyun.cn

[Q85] 数值取整
来源：http://jek.chenjidiqi.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aie.pycfn.com

[Q86] 读取 JSON 字段
来源：http://mjc.jiagoushi.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vcb.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://oei.daxiang520.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ufo.xylfe.cn

[Q88] 行转列（条件聚合）
来源：http://mjl.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://izu.guannengcc.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dwd.zdbjq.cn

[Q89] 判断表是否存在
来源：http://rwo.hnxiangtu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ccu.hammf.cn

[Q90] 生成序号列
来源：http://lxb.bjfxy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://qao.52xcode.cn

================================================================================
来源：http://hnl.hongshengwenyu.top

R. Bash 专题
来源：http://psr.iojbl.cn

================================================================================
来源：http://yno.zhongyouzk.top

[R01] shebang 与严格模式
来源：http://gnw.shzxlz.cn

#!/usr/bin/env bash
来源：http://jit.jinqigufen.top

set -euo pipefail
来源：http://tkk.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://ggx.tianlin.xyz

name="Tom"; echo "$name"
来源：http://yfa.chenjidiqi.icu

[R03] 只读变量
来源：http://vln.havefunace.top

readonly PI=3.14
来源：http://uso.yuanzhike.top

[R04] 位置参数
来源：http://pea.ydjk.org.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://bic.c1oappe.top

[R05] 参数默认值
来源：http://sow.sufxvd.cn

name="${1:-default}"
来源：http://dhc.pycfn.com

[R06] 判断命令是否存在
来源：http://jle.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mlq.hongshengwenyu.top

[R07] if 判断文件
来源：http://auh.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://spn.zhoulong.xyz

[R08] 数值比较
来源：http://fqr.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nhz.ctjpmb.com

[R09] 字符串比较
来源：http://ffi.chenjidiqi.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wsz.fanxiaobao.xyz

[R10] 正则匹配
来源：http://wdu.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vky.cheryme.top

[R11] case 多分支
来源：http://mgn.jiagoushi.top

case "$1" in
来源：http://lje.hysaishi.cn

start) echo "启动" ;;
来源：http://gou.yuxming.cn

stop)  echo "停止" ;;
来源：http://vwh.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://ynu.shanyushiyangtech.top

esac
来源：http://wwp.xinyue.icu

[R12] for 遍历文件
来源：http://mvy.haohaochexian.top

for f in *.txt; do echo "$f"; done
来源：http://dxh.tian-w.cn

[R13] for 计数循环
来源：http://tbo.316326.xyz

for i in {1..10}; do echo "$i"; done
来源：http://xkd.zycfv.cn

[R14] C 风格 for
来源：http://lbn.zdbjq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qkd.hywenlv.cn

[R15] while 逐行读文件
来源：http://slb.ppjwa.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wsk.yueranfly.top

[R16] until 等待条件
来源：http://bvw.sweek.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://suj.bjfxy.top

[R17] 数组定义与取值
来源：http://dib.tanke756.top

arr=(a b c); echo "${arr[0]}"
来源：http://gjx.52xcode.cn

[R18] 遍历数组
来源：http://zpb.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qms.meibo888.top

[R19] 数组长度
来源：http://edh.redwolf501.top

echo "${#arr[@]}"
来源：http://pcu.nwbrower.top

[R20] 关联数组（字典）
来源：http://jdw.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://veg.redwolf501.top

[R21] 字符串长度
来源：http://ugl.xuanzx.com

echo "${#s}"
来源：http://cbz.yj20258.top

[R22] 截取子串
来源：http://bem.hywenlv.cn

echo "${s:0:5}"
来源：http://fxz.ybcxt.top

[R23] 字符串替换
来源：http://myt.yj20258888.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://txq.shanyushiyangtech.top

[R24] 大小写转换
来源：http://fon.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://opa.shangyingyoupin.top

[R25] 去后缀 / 去前缀
来源：http://uua.yj202588.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tkk.pycfn.com

[R26] 命令替换
来源：http://vhm.zdbjq.cn

now=$(date +%F); echo "$now"
来源：http://ruc.ppjwa.cn

[R27] 算术展开
来源：http://vmr.ywan-chungtsiang.top

echo $((1 + 2 * 3))
来源：http://owl.sxryk.cn

[R28] 浮点运算
来源：http://spy.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://zvh.xziqi.cn

[R29] 定义函数
来源：http://kwr.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sbv.ydjk.org.cn

[R30] 函数返回状态码
来源：http://dck.sxryk.cn

f() { return 0; }; f || echo "失败了"
来源：http://mhc.9152youxi.cn

[R31] 局部变量
来源：http://sbb.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://mcy.shangyingyoupin.top

[R32] 参数个数校验
来源：http://xeg.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lfw.yuanzhike.top

[R33] 捕获错误并提示行号
来源：http://dmx.uphjek.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sdx.fehbvm.com

[R34] 退出时清理
来源：http://nsy.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://pww.nwbrower.top

[R35] 后台执行并等待
来源：http://rfn.uphjek.com

sleep 5 & pid=$!; wait "$pid"
来源：http://ksd.zhongyouzk.top

[R36] 并发执行多个任务
来源：http://drv.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kre.xziqi.cn

[R37] 把输出赋给变量
来源：http://nsc.ydjk.org.cn

files=$(ls -1)
来源：http://lux.jinqigfzy.top

[R38] 管道串联
来源：http://wre.hesvh.cn

cat a.txt | grep -i error | wc -l
来源：http://scv.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://lfg.svipenyu.cn

cmd > out.log 2>&1
来源：http://clh.vqdsnc.cn

[R40] 追加写日志
来源：http://oxr.birdmap.top

echo "log" >> out.log
来源：http://ann.sjlbkw.cn

[R41] 丢弃输出
来源：http://jnu.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://qmc.yj20258.top

[R42] 输入重定向
来源：http://ymb.dianchejie.cn

wc -l < a.txt
来源：http://prt.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://nsg.zdqjudy.top

find . -name "*.log" -type f
来源：http://aac.0kj1m.cn

[R44] 按修改时间查找
来源：http://nmk.gogol.net.cn

find . -mtime -7 -type f
来源：http://rxx.shanyushiyangtech.top

[R45] 批量删除
来源：http://gay.jqgfzy.top

find . -name "*.tmp" -delete
来源：http://rba.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://lyx.xingfuxueyuan.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fif.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://xyk.havefunace.top

sed -i 's/foo/bar/g' a.txt
来源：http://uav.316326.xyz

[R48] awk 取指定列
来源：http://flt.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://niq.cdnleiting.top

[R49] awk 带条件
来源：http://xbf.feifeiyinyue.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ykt.9152youxi.cn

[R50] awk 求和
来源：http://yas.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://lym.quarkkingdee.top

[R51] 排序去重取前几
来源：http://cth.daria6918.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qic.jiagoushi.top

[R52] 统计行数
来源：http://vlz.yangfankeji.com

wc -l a.txt
来源：http://lez.ybcxt.top

[R53] 查看文件头与实时尾
来源：http://wib.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://yib.pengpengdd.cyou

[R54] 比较两个文件
来源：http://ssw.pycfn.com

diff a.txt b.txt
来源：http://igf.ywan-chungtsiang.top

[R55] 压缩与解压
来源：http://fzl.wangdashe.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://auq.xuetiantiany.cn

[R56] 远程拷贝
来源：http://acj.sxryk.cn

scp file user@host:/path/
来源：http://abc.cqqwz.cn

[R57] 远程执行命令
来源：http://bsp.shuidangran.top

ssh user@host 'uptime'
来源：http://rer.havefunace.top

[R58] 下载文件
来源：http://oig.jinyuanbaomall.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bcv.fengsongda.top

[R59] 发 POST JSON
来源：http://hlz.iojbl.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://osr.zdbjq.cn

[R60] 只看 HTTP 状态码
来源：http://gqb.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bax.svipenyu.cn

[R61] 磁盘占用
来源：http://poj.zhijiandao.cn

df -h;  du -sh *
来源：http://aka.hysaishi.cn

[R62] 找最占空间的文件
来源：http://lme.hammf.cn

du -ah . | sort -rh | head -10
来源：http://zmq.hfpthk.cn

[R63] 内存与进程
来源：http://imk.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://tpw.c1oappe.top

[R64] 结束进程
来源：http://ckv.hammf.cn

kill -9 $(pgrep -f app.py)
来源：http://via.quarkkingdee.top

[R65] 查看端口占用
来源：http://lqh.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nem.uphjek.com

[R66] 定时任务
来源：http://nso.tianlin.xyz

crontab -e;  crontab -l
来源：http://oei.jianghu66.top

[R67] 生成随机十六进制串
来源：http://rod.zhoulong.xyz

openssl rand -hex 16
来源：http://bdz.hammf.cn

[R68] 计算文件校验值
来源：http://qgq.iojbl.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uux.quarkkingdee.top

[R69] 生成随机密码
来源：http://eyx.fehbvm.com

head -c 16 /dev/urandom | base64
来源：http://tnl.hywenlv.cn

[R70] 时间戳与互转
来源：http://wxw.xuanzx.com

date +%s;  date -d @1700000000
来源：http://qng.mhx1999.top

[R71] 日期格式化
来源：http://fse.tanke756.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://web.sxryk.cn

[R72] 等待端口就绪
来源：http://wxg.yj20258.top

until nc -z localhost 3306; do sleep 1; done
来源：http://anp.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://bsr.yonumen.top

split -l 1000 big.log part_
来源：http://xpn.birdmap.top

[R74] 批量重命名
来源：http://qlt.bbcook.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iup.xuetiantiany.cn

[R75] 导出环境变量
来源：http://nif.zhoulong.xyz

export PATH="$HOME/bin:$PATH"
来源：http://elo.ivvv.top

[R76] 使用临时文件
来源：http://zic.xziqi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xuh.shzxlz.cn

[R77] 读取用户输入
来源：http://fsi.316326.xyz

read -rp "请输入: " ans
来源：http://xxk.gzhubu.top

[R78] 交互式菜单
来源：http://tgl.yueranfly.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qus.yonumen.top

[R79] 解析命令行选项
来源：http://wmk.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xvb.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://nsp.sweek.top

time ./run.sh
来源：http://yuk.jinqigufen.top

================================================================================
来源：http://iid.316326.xyz

S. C / C++ 专题
来源：http://isi.ydjk.org.cn

================================================================================
来源：http://lrz.xylfe.cn

[S01] C：Hello World
来源：http://zzm.haohaochexian.top

#include <stdio.h>
来源：http://nte.yj202588.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://kzj.hcnkem.com

[S02] C：变量与格式化输出
来源：http://axq.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://yng.feifeiyinyue.top

[S03] C：读入整数
来源：http://hxm.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://oji.dashuyun.cn

[S04] C：字符串复制
来源：http://lxu.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://zjk.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://dah.aibaodan.cn

strlen(s)
来源：http://bav.xuanzx.com

[S06] C：字符串比较
来源：http://fac.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://rsy.jinqigufen.top

[S07] C：数组遍历求和
来源：http://cgo.hcnkem.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bnw.jinghuilouyu.cn

[S08] C：动态内存分配与释放
来源：http://cje.gzhubu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xjo.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://ffd.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iyj.316326.xyz

[S10] C：指针与解引用
来源：http://frz.yuxming.cn

int *p = &a;  *p = 5;
来源：http://nke.andypj.xyz

[S11] C：逐行读文件
来源：http://enc.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://tjw.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hcz.gaohongyu789.top

fclose(f);
来源：http://hzk.xingfuxueyuan.xyz

[S12] C：写文件
来源：http://uep.xuanzx.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://reb.jianghu66.top

[S13] C：宏定义
来源：http://ziy.gzhubu.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tnh.jiagoushi.top

[S14] C：枚举
来源：http://uql.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://apb.gzhubu.top

[S15] C：类型转换
来源：http://syf.ppjwa.cn

(double) a / b
来源：http://cbp.yuxming.cn

[S16] C：位操作置位
来源：http://lhc.c1oappe.top

x |= (1 << 3);
来源：http://tog.316326.xyz

[S17] C：安全拼接字符串
来源：http://cak.yj20258888.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lic.sweek.top

[S18] C：命令行参数
来源：http://shv.tarul.cn

int main(int argc, char **argv)
来源：http://wtr.shangyingyoupin.top

[S19] C：快速排序
来源：http://avf.uphjek.com

qsort(a, n, sizeof(int), cmp);
来源：http://krp.jinghuilouyu.cn

[S20] C：二分查找
来源：http://nsu.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uhj.zdbjq.cn

[S21] C：字符类别判断
来源：http://glb.xinyue.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vdp.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://gst.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://ulh.9152youxi.cn

[S23] C：随机数
来源：http://bul.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wli.zhaomingkeji.xyz

[S24] C：获取本地时间
来源：http://xao.yj20258888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jsf.zhixingplan.top

[S25] C：内存拷贝
来源：http://wrw.yuanzhike.top

memcpy(dst, src, n);
来源：http://rli.epnwcf.com

[S26] C：内存清零
来源：http://xqv.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://ymq.yuanzhike.top

[S27] C：定义常量
来源：http://cfj.yonumen.top

const double PI = 3.14159;
来源：http://qao.hesvh.cn

[S28] C：静态变量
来源：http://lze.tian-w.cn

static int counter = 0;
来源：http://ezu.ppjwa.cn

[S29] C：变参函数
来源：http://nda.birdmap.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rvs.c1oappe.top

[S30] C：头文件保护
来源：http://opr.yangfankeji.com

#ifndef X_H
来源：http://ycg.snrcjt.cn

#define X_H
来源：http://dsk.shangyingyoupin.top

#endif
来源：http://eox.zhengqikj.top

[S31] C++：Hello World
来源：http://miy.shangyingyoupin.top

#include <iostream>
来源：http://fkg.fktsv.cn

int main() { std::cout << "Hello\n"; }
来源：http://dxd.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://fyu.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://eww.nanxinkj.top

[S33] C++：vector 增删
来源：http://rru.jlsjyb.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cvv.tian-w.cn

[S34] C++：遍历 vector
来源：http://kkq.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://yay.iojbl.cn

[S35] C++：map
来源：http://qlx.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gxy.havefunace.top

[S36] C++：unordered_map
来源：http://lkp.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lgi.yfazqb.com

[S37] C++：set
来源：http://eej.bbcook.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ohm.jinqigfzy.top

[S38] C++：排序
来源：http://nyr.dianchejie.cn

std::sort(v.begin(), v.end());
来源：http://udy.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://uip.fanxiaobao.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qhk.haohaochexian.top

[S40] C++：查找元素
来源：http://omf.tian-w.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://occ.zhengqikj.top

[S41] C++：类与构造函数
来源：http://mgm.iojbl.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xkx.kuanghao11.cn

[S42] C++：继承与虚函数
来源：http://qds.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://lfc.hesvh.cn

[S43] C++：智能指针
来源：http://bql.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://qtv.jqgufenzy.top

[S44] C++：引用传参
来源：http://fki.guannengcc.top

void inc(int &x) { ++x; }
来源：http://aux.ppjwa.cn

[S45] C++：lambda
来源：http://ugr.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://hcm.shanyushiyangkeji.top

[S46] C++：函数模板
来源：http://why.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vor.vehdjk.com

[S47] C++：结构化绑定遍历
来源：http://hpi.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://efv.jyoumei.cn

[S48] C++：逐行读文件
来源：http://ync.shzxlz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://egg.uphjek.com

while (std::getline(in, line)) { }
来源：http://gaq.cucudq.cn

[S49] C++：写文件
来源：http://yud.yongpay.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ffj.zdbjq.cn

[S50] C++：格式化数字
来源：http://gad.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mgc.fzhhl.top

[S51] C++：显式类型转换
来源：http://vue.mhx1999.top

static_cast<double>(a) / b
来源：http://obb.redwolf501.top

[S52] C++：const 与 noexcept
来源：http://gbk.gaohongyu789.top

int size() const noexcept { return n_; }
来源：http://ijd.yj202588.top

[S53] C++：移动语义
来源：http://ymu.tanke756.top

std::vector<int> w = std::move(v);
来源：http://pdg.cqqwz.cn

[S54] C++：异常处理
来源：http://zlo.yueranfly.top


<!-- 参考信息 -->