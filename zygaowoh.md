代发 wailian999

[Q82] 字符长度与字节长度
来源：http://zmc.epnwcf.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ufc.quarkkingdee.top

[Q83] 大小写转换
来源：http://hdq.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://gun.cdnleiting.top

[Q84] 去除首尾空格
来源：http://zpb.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://zfh.wangdashe.top

[Q85] 数值取整
来源：http://wuv.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://sfd.nanxuanxn.top

[Q86] 读取 JSON 字段
来源：http://wfd.bjfxy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dxd.shuidangran.top

[Q87] JSON 字段做条件
来源：http://mgg.cucudq.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mau.shangyingyoupin.top

[Q88] 行转列（条件聚合）
来源：http://jvc.dashuyun.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zfv.hongshengwenyu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vtk.zdbjq.cn

[Q89] 判断表是否存在
来源：http://glw.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tmx.316326.xyz

[Q90] 生成序号列
来源：http://wkv.jinqigufen.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wmv.hysaishi.cn

================================================================================
来源：http://ovr.cdnleiting.top

R. Bash 专题
来源：http://ovb.snrcjt.cn

================================================================================
来源：http://xzj.ivvv.top

[R01] shebang 与严格模式
来源：http://mmn.yj20258.top

#!/usr/bin/env bash
来源：http://cme.ydzc1.top

set -euo pipefail
来源：http://kqk.epnwcf.com

[R02] 变量赋值与使用
来源：http://ntr.zhongyouzk.top

name="Tom"; echo "$name"
来源：http://aqh.gaohongyu789.top

[R03] 只读变量
来源：http://hqe.dashuyun.cn

readonly PI=3.14
来源：http://lph.haohaochexian.top

[R04] 位置参数
来源：http://fmw.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xml.sufxvd.cn

[R05] 参数默认值
来源：http://try.tian-w.cn

name="${1:-default}"
来源：http://ixi.shzxlz.cn

[R06] 判断命令是否存在
来源：http://fpw.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lpa.bbcook.cn

[R07] if 判断文件
来源：http://rmw.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hut.sweek.top

[R08] 数值比较
来源：http://knt.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://unv.gaohongyu789.top

[R09] 字符串比较
来源：http://phy.hysaishi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cty.xziqi.cn

[R10] 正则匹配
来源：http://pyz.epnwcf.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://krk.nanxinkj.top

[R11] case 多分支
来源：http://ehz.xinyue.icu

case "$1" in
来源：http://ouf.andypj.xyz

start) echo "启动" ;;
来源：http://yhh.wangdashe.top

stop)  echo "停止" ;;
来源：http://odu.zhiwuduotai.top

*)     echo "未知命令" ;;
来源：http://zex.9152youxi.cn

esac
来源：http://vps.jyoumei.cn

[R12] for 遍历文件
来源：http://rnz.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://aaw.guowangkeji.top

[R13] for 计数循环
来源：http://dqg.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://yua.jinqigufen.top

[R14] C 风格 for
来源：http://bpy.fehbvm.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zsd.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://ogy.zhijiandao.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdz.smart0.xyz

[R16] until 等待条件
来源：http://viu.vqdsnc.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vjm.meibo888.top

[R17] 数组定义与取值
来源：http://lqb.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://oju.ydjk.org.cn

[R18] 遍历数组
来源：http://psj.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ewl.ppjwa.cn

[R19] 数组长度
来源：http://hwl.shzxlz.cn

echo "${#arr[@]}"
来源：http://cxr.pengpengdd.cyou

[R20] 关联数组（字典）
来源：http://tra.52xcode.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sjm.aizwys.cn

[R21] 字符串长度
来源：http://imy.epnwcf.com

echo "${#s}"
来源：http://cnk.iojbl.cn

[R22] 截取子串
来源：http://toi.sufxvd.cn

echo "${s:0:5}"
来源：http://rnz.gogol.net.cn

[R23] 字符串替换
来源：http://zbc.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rmk.yongpay.top

[R24] 大小写转换
来源：http://fvs.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://gjk.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://ftp.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ons.jinqigfzy.top

[R26] 命令替换
来源：http://fkp.zhijiandao.cn

now=$(date +%F); echo "$now"
来源：http://ijr.yuanzhike.top

[R27] 算术展开
来源：http://zfq.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://mhl.ehwqpu.com

[R28] 浮点运算
来源：http://txw.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://qqd.yueranfly.top

[R29] 定义函数
来源：http://zpq.ivvv.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ain.sjlbkw.cn

[R30] 函数返回状态码
来源：http://miy.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://ojm.sweek.top

[R31] 局部变量
来源：http://neg.fengsongda.top

f() { local x=1; echo "$x"; }
来源：http://nvf.aizwys.cn

[R32] 参数个数校验
来源：http://gqj.fehbvm.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://krm.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://gqj.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yiw.wangshuangyany.cn

[R34] 退出时清理
来源：http://axi.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jqp.yangfankeji.com

[R35] 后台执行并等待
来源：http://jxl.xinyue.icu

sleep 5 & pid=$!; wait "$pid"
来源：http://kxs.hammf.cn

[R36] 并发执行多个任务
来源：http://oub.sufxvd.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://szn.zdbjq.cn

[R37] 把输出赋给变量
来源：http://xpr.zhaomingkeji.xyz

files=$(ls -1)
来源：http://udp.jyoumei.cn

[R38] 管道串联
来源：http://gka.tian-w.cn

cat a.txt | grep -i error | wc -l
来源：http://jrq.shangyingyoupin.top

[R39] 重定向标准输出与错误
来源：http://har.jiagoushi.top

cmd > out.log 2>&1
来源：http://ztr.hcnkem.com

[R40] 追加写日志
来源：http://oxh.vehdjk.com

echo "log" >> out.log
来源：http://exq.xuetiantiany.cn

[R41] 丢弃输出
来源：http://nvg.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://bvt.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://yrv.uphjek.com

wc -l < a.txt
来源：http://xmi.chenlongwang.top

[R43] 按名字查找文件
来源：http://egw.aizwys.cn

find . -name "*.log" -type f
来源：http://nhk.zycfv.cn

[R44] 按修改时间查找
来源：http://lpn.vqdsnc.cn

find . -mtime -7 -type f
来源：http://cnd.cucudq.cn

[R45] 批量删除
来源：http://eqi.xziqi.cn

find . -name "*.tmp" -delete
来源：http://mot.daria6918.cn

[R46] 递归替换文件内容
来源：http://unm.zycfv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uhp.nanxuanxn.top

[R47] sed 单行替换
来源：http://uft.wangshuangyany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wur.zhongyouzk.top

[R48] awk 取指定列
来源：http://kgt.0kj1m.cn

awk '{print $1, $3}' a.txt
来源：http://qda.cheryme.top

[R49] awk 带条件
来源：http://pha.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://czy.tarul.cn

[R50] awk 求和
来源：http://xzg.iojbl.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fnf.kuanghao11.cn

[R51] 排序去重取前几
来源：http://zhn.svipenyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qkj.fengsongda.top

[R52] 统计行数
来源：http://fds.sweek.top

wc -l a.txt
来源：http://mjm.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://pqu.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ajf.fzhhl.top

[R54] 比较两个文件
来源：http://gjx.hammf.cn

diff a.txt b.txt
来源：http://mmr.jinqigfzy.top

[R55] 压缩与解压
来源：http://mjd.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://imu.hammf.cn

[R56] 远程拷贝
来源：http://qsw.vehdjk.com

scp file user@host:/path/
来源：http://hse.nanxinkj.top

[R57] 远程执行命令
来源：http://ayy.cqqwz.cn

ssh user@host 'uptime'
来源：http://jcu.tarul.cn

[R58] 下载文件
来源：http://dvx.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yrf.ehwqpu.com

[R59] 发 POST JSON
来源：http://rmo.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://oei.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://zen.gaohongyu789.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://srl.ctjpmb.com

[R61] 磁盘占用
来源：http://fwd.hcnkem.com

df -h;  du -sh *
来源：http://ovh.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://ztq.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://lsh.redwolf501.top

[R63] 内存与进程
来源：http://jwb.sxryk.cn

free -h;  ps aux | grep nginx
来源：http://qsy.aizwys.cn

[R64] 结束进程
来源：http://pqx.pycfn.com

kill -9 $(pgrep -f app.py)
来源：http://aam.zhengqikj.top

[R65] 查看端口占用
来源：http://aad.shanyushiyangkeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kmk.shzxlz.cn

[R66] 定时任务
来源：http://hjv.nanxinkj.top

crontab -e;  crontab -l
来源：http://zgj.sxryk.cn

[R67] 生成随机十六进制串
来源：http://exa.aizwys.cn

openssl rand -hex 16
来源：http://uex.hnqzz.top

[R68] 计算文件校验值
来源：http://rth.gaohongyu789.top

sha256sum a.txt;  md5sum a.txt
来源：http://jwb.andypj.xyz

[R69] 生成随机密码
来源：http://ijt.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://ygo.nwbrower.top

[R70] 时间戳与互转
来源：http://iyo.yueranfly.top

date +%s;  date -d @1700000000
来源：http://nfu.gotoacloud.top

[R71] 日期格式化
来源：http://piz.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lum.yongpay.top

[R72] 等待端口就绪
来源：http://bzp.svipenyu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qod.yongpay.top

[R73] 分割大日志
来源：http://tfn.316326.xyz

split -l 1000 big.log part_
来源：http://dyj.fktsv.cn

[R74] 批量重命名
来源：http://bcq.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqg.jianghu66.top

[R75] 导出环境变量
来源：http://axl.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://ptg.vehdjk.com

[R76] 使用临时文件
来源：http://tbp.yangfankeji.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ebe.tianlin.xyz

[R77] 读取用户输入
来源：http://mai.yuxming.cn

read -rp "请输入: " ans
来源：http://fmf.jqgufenzy.top

[R78] 交互式菜单
来源：http://tjd.0kj1m.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hjf.dianchejie.cn

[R79] 解析命令行选项
来源：http://yqh.birdmap.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ffd.guannengcc.top

[R80] 查看脚本执行耗时
来源：http://mpv.hesvh.cn

time ./run.sh
来源：http://unb.jinghuilouyu.cn

================================================================================
来源：http://hfd.sweek.top

S. C / C++ 专题
来源：http://rto.jianghu66.top

================================================================================
来源：http://hqj.jlsjyb.cn

[S01] C：Hello World
来源：http://tyj.jianghu66.top

#include <stdio.h>
来源：http://jvz.quarkkingdee.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jhn.hammf.cn

[S02] C：变量与格式化输出
来源：http://euj.ehwqpu.com

int a = 10; printf("%d\n", a);
来源：http://yzm.hcnkem.com

[S03] C：读入整数
来源：http://bly.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://ydo.sufxvd.cn

[S04] C：字符串复制
来源：http://xmu.chenlongwang.top

char dst[32]; strcpy(dst, "hi");
来源：http://nly.meibo888.top

[S05] C：字符串长度
来源：http://jsd.quarkkingdee.top

strlen(s)
来源：http://cni.hnxiangtu.top

[S06] C：字符串比较
来源：http://ttq.guowangkeji.top

strcmp(a, b) == 0
来源：http://ikx.hcnkem.com

[S07] C：数组遍历求和
来源：http://oas.zdqjudy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://swu.jinyuanbaomall.cn

[S08] C：动态内存分配与释放
来源：http://lmm.hfpthk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tgc.yuanzhike.top

[S09] C：结构体定义与初始化
来源：http://xjr.hfpthk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://riz.vehdjk.com

[S10] C：指针与解引用
来源：http://bzu.yanxiufei.cn

int *p = &a;  *p = 5;
来源：http://gnp.yuanzhike.top

[S11] C：逐行读文件
来源：http://dkh.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://tor.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://aqk.bjfxy.top

fclose(f);
来源：http://ott.yuxming.cn

[S12] C：写文件
来源：http://bbn.tian-w.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zpn.shangyingyoupin.top

[S13] C：宏定义
来源：http://feo.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eup.meibo888.top

[S14] C：枚举
来源：http://mao.xuetiantiany.cn

enum Color { RED, GREEN, BLUE };
来源：http://aia.shangyingyoupin.top

[S15] C：类型转换
来源：http://bdp.fengsongda.top

(double) a / b
来源：http://wfm.xuetiantiany.cn

[S16] C：位操作置位
来源：http://upb.nwbrower.top

x |= (1 << 3);
来源：http://vss.ivvv.top

[S17] C：安全拼接字符串
来源：http://ftd.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://acm.jinghuilouyu.cn

[S18] C：命令行参数
来源：http://ioh.yuanzhike.top

int main(int argc, char **argv)
来源：http://yoh.gogol.net.cn

[S19] C：快速排序
来源：http://plb.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://hys.shuidangran.top

[S20] C：二分查找
来源：http://urw.c1oappe.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hdh.tianlin.xyz

[S21] C：字符类别判断
来源：http://emc.cashguo.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rxd.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://jbf.havefunace.top

atoi("42");  strtod("3.14", NULL);
来源：http://fnu.hysaishi.cn

[S23] C：随机数
来源：http://rwo.epnwcf.com

srand(time(NULL));  int r = rand() % 100;
来源：http://xsr.sjlbkw.cn

[S24] C：获取本地时间
来源：http://xtm.daxiang520.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nnw.9152youxi.cn

[S25] C：内存拷贝
来源：http://uqs.zhiwuduotai.top

memcpy(dst, src, n);
来源：http://wpb.ivvv.top

[S26] C：内存清零
来源：http://pnq.jianghu66.top

memset(a, 0, sizeof a);
来源：http://mdd.tian-w.cn

[S27] C：定义常量
来源：http://jto.wangshuangyany.cn

const double PI = 3.14159;
来源：http://cdz.zdqjudy.top

[S28] C：静态变量
来源：http://guz.sweek.top

static int counter = 0;
来源：http://hun.haohaochexian.top

[S29] C：变参函数
来源：http://hul.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iah.yanxiufei.cn

[S30] C：头文件保护
来源：http://okz.hysaishi.cn

#ifndef X_H
来源：http://ngv.fanxiaobao.xyz

#define X_H
来源：http://ltl.xziqi.cn

#endif
来源：http://iwo.sxryk.cn

[S31] C++：Hello World
来源：http://wtq.xuetiantiany.cn

#include <iostream>
来源：http://bgu.zhiwuduotai.top

int main() { std::cout << "Hello\n"; }
来源：http://gqt.jqgufenzy.top

[S32] C++：字符串
来源：http://uak.mhx1999.top

std::string s = "hi";  s += "!";
来源：http://usg.mhx1999.top

[S33] C++：vector 增删
来源：http://mhw.tianlin.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kph.ehwqpu.com

[S34] C++：遍历 vector
来源：http://rbe.tarul.cn

for (auto &x : v) { std::cout << x; }
来源：http://txb.cqqwz.cn

[S35] C++：map
来源：http://knx.kuanghao11.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sja.gzhubu.top

[S36] C++：unordered_map
来源：http://ppo.sjlbkw.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rpf.xuanzx.com

[S37] C++：set
来源：http://hmg.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xbs.svipenyu.cn

[S38] C++：排序
来源：http://brt.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://yaq.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://ezg.svipenyu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vmk.jinqigufen.top

[S40] C++：查找元素
来源：http://blw.mhx1999.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cjl.zhixingplan.top

[S41] C++：类与构造函数
来源：http://itn.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gmp.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://zbe.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://ppp.hnqzz.top

[S43] C++：智能指针
来源：http://gvg.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://dth.snrcjt.cn

[S44] C++：引用传参
来源：http://vdq.dashuyun.cn

void inc(int &x) { ++x; }
来源：http://jrq.hysaishi.cn

[S45] C++：lambda
来源：http://ecw.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fht.yuxming.cn

[S46] C++：函数模板
来源：http://zna.hesvh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jug.iojbl.cn

[S47] C++：结构化绑定遍历
来源：http://tlp.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fzn.zdqjudy.top

[S48] C++：逐行读文件
来源：http://alb.bbcook.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sdo.tianlin.xyz

while (std::getline(in, line)) { }
来源：http://kpv.ehwqpu.com

[S49] C++：写文件
来源：http://hcz.yvedp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wob.jinqigfzy.top

[S50] C++：格式化数字
来源：http://mup.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dbr.guowangkeji.top

[S51] C++：显式类型转换
来源：http://mma.yvedp.cn

static_cast<double>(a) / b
来源：http://vqw.aizwys.cn

[S52] C++：const 与 noexcept
来源：http://awn.hnqzz.top


<!-- 参考信息 -->