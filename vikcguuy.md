代发 wailian999

[Q86] 读取 JSON 字段
来源：http://iqw.dianchejie.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://kmf.jinqigfzy.top

[Q87] JSON 字段做条件
来源：http://hop.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fwz.xingfuxueyuan.xyz

[Q88] 行转列（条件聚合）
来源：http://vgm.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pap.snrcjt.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ebc.gzhubu.top

[Q89] 判断表是否存在
来源：http://csj.fehbvm.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://tlj.tianlin.xyz

[Q90] 生成序号列
来源：http://xqi.dashuyun.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bhh.yongpay.top

================================================================================
来源：http://dbf.ydzc1.top

R. Bash 专题
来源：http://cqt.c1oappe.top

================================================================================
来源：http://sjh.dashuyun.cn

[R01] shebang 与严格模式
来源：http://flb.ehwqpu.com

#!/usr/bin/env bash
来源：http://nep.hongshengwenyu.top

set -euo pipefail
来源：http://uza.nanxuanxn.top

[R02] 变量赋值与使用
来源：http://htn.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://yga.zhoulong.xyz

[R03] 只读变量
来源：http://zvk.zhiwuduotai.top

readonly PI=3.14
来源：http://qlv.yj20258888.top

[R04] 位置参数
来源：http://pbr.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qth.hysaishi.cn

[R05] 参数默认值
来源：http://dqm.ppjwa.cn

name="${1:-default}"
来源：http://dez.pengpengdd.cyou

[R06] 判断命令是否存在
来源：http://ajb.yanxiufei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hpa.pengpengdd.cyou

[R07] if 判断文件
来源：http://flx.hammf.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ilv.ehwqpu.com

[R08] 数值比较
来源：http://nkd.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dep.quarkkingdee.top

[R09] 字符串比较
来源：http://dna.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://czd.jqgfzy.top

[R10] 正则匹配
来源：http://bop.sufxvd.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sjw.shanyushiyangtech.top

[R11] case 多分支
来源：http://mvw.kuanghao11.cn

case "$1" in
来源：http://izt.yvedp.cn

start) echo "启动" ;;
来源：http://dmv.hysaishi.cn

stop)  echo "停止" ;;
来源：http://xjp.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://ixg.jqgufenzy.top

esac
来源：http://frl.ehwqpu.com

[R12] for 遍历文件
来源：http://hge.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://qpk.quarkkingdee.top

[R13] for 计数循环
来源：http://ijg.jinyuanbaomall.cn

for i in {1..10}; do echo "$i"; done
来源：http://qop.jianghu66.top

[R14] C 风格 for
来源：http://pie.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jzq.jianghu66.top

[R15] while 逐行读文件
来源：http://uqt.zdqjudy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jfy.chenlongwang.top

[R16] until 等待条件
来源：http://oyi.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yrr.jinqigfzy.top

[R17] 数组定义与取值
来源：http://rvw.shanyushiyangtech.top

arr=(a b c); echo "${arr[0]}"
来源：http://rom.gogol.net.cn

[R18] 遍历数组
来源：http://nus.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gjm.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://snf.aibaodan.cn

echo "${#arr[@]}"
来源：http://xvu.fehbvm.com

[R20] 关联数组（字典）
来源：http://wij.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://reb.hcnkem.com

[R21] 字符串长度
来源：http://ong.hammf.cn

echo "${#s}"
来源：http://sut.andypj.xyz

[R22] 截取子串
来源：http://dfx.sxryk.cn

echo "${s:0:5}"
来源：http://fxq.0kj1m.cn

[R23] 字符串替换
来源：http://mwy.nwbrower.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rkn.yuxming.cn

[R24] 大小写转换
来源：http://adr.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://rms.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://wba.vqdsnc.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://jft.quarkkingdee.top

[R26] 命令替换
来源：http://zfa.zdqjudy.top

now=$(date +%F); echo "$now"
来源：http://toa.yj202588.top

[R27] 算术展开
来源：http://jlm.svipenyu.cn

echo $((1 + 2 * 3))
来源：http://lmb.fzhhl.top

[R28] 浮点运算
来源：http://bzd.zhongyouzk.top

echo "scale=2; 10/3" | bc
来源：http://heq.yuxming.cn

[R29] 定义函数
来源：http://hot.jinqigfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zjs.zhijiandao.cn

[R30] 函数返回状态码
来源：http://bco.hesvh.cn

f() { return 0; }; f || echo "失败了"
来源：http://tlr.zdqjudy.top

[R31] 局部变量
来源：http://zqo.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://fmq.sjlbkw.cn

[R32] 参数个数校验
来源：http://vnn.sjlbkw.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ggj.tanke756.top

[R33] 捕获错误并提示行号
来源：http://xcv.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jxg.aizwys.cn

[R34] 退出时清理
来源：http://uha.tianlin.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://ece.wangshuangyany.cn

[R35] 后台执行并等待
来源：http://hvv.jiagoushi.top

sleep 5 & pid=$!; wait "$pid"
来源：http://wbd.yj20258888.top

[R36] 并发执行多个任务
来源：http://tgu.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ebp.smart0.xyz

[R37] 把输出赋给变量
来源：http://vpc.xinyue.icu

files=$(ls -1)
来源：http://nip.redwolf501.top

[R38] 管道串联
来源：http://pit.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://rqe.sweek.top

[R39] 重定向标准输出与错误
来源：http://yra.yongpay.top

cmd > out.log 2>&1
来源：http://tfe.cucudq.cn

[R40] 追加写日志
来源：http://eoo.dashuyun.cn

echo "log" >> out.log
来源：http://cra.yueranfly.top

[R41] 丢弃输出
来源：http://pcy.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://jnj.cucudq.cn

[R42] 输入重定向
来源：http://cyj.yongpay.top

wc -l < a.txt
来源：http://lox.c1oappe.top

[R43] 按名字查找文件
来源：http://jki.pycfn.com

find . -name "*.log" -type f
来源：http://vdm.hnqzz.top

[R44] 按修改时间查找
来源：http://tuw.iojbl.cn

find . -mtime -7 -type f
来源：http://waf.jyoumei.cn

[R45] 批量删除
来源：http://hbk.sysykeji.top

find . -name "*.tmp" -delete
来源：http://npt.tarul.cn

[R46] 递归替换文件内容
来源：http://fcp.snrcjt.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qyx.fengsongda.top

[R47] sed 单行替换
来源：http://krp.chenlongwang.top

sed -i 's/foo/bar/g' a.txt
来源：http://hhx.yongpay.top

[R48] awk 取指定列
来源：http://nyu.haohaochexian.top

awk '{print $1, $3}' a.txt
来源：http://cnk.sweek.top

[R49] awk 带条件
来源：http://auy.yongpay.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eiy.yj20258888.top

[R50] awk 求和
来源：http://guz.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cka.yfazqb.com

[R51] 排序去重取前几
来源：http://puf.tian-w.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://taa.feifeiyinyue.top

[R52] 统计行数
来源：http://evs.sxryk.cn

wc -l a.txt
来源：http://tit.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://gnx.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iwe.chenzaomai.com

[R54] 比较两个文件
来源：http://voj.gotoacloud.top

diff a.txt b.txt
来源：http://xza.quarkkingdee.top

[R55] 压缩与解压
来源：http://bsq.kuanghao11.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jqh.gogol.net.cn

[R56] 远程拷贝
来源：http://xms.quarkkingdee.top

scp file user@host:/path/
来源：http://tpn.jyoumei.cn

[R57] 远程执行命令
来源：http://taj.chenlongwang.top

ssh user@host 'uptime'
来源：http://sav.pengpengdd.cyou

[R58] 下载文件
来源：http://cmw.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kfg.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://vzs.cheryme.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iuq.tarul.cn

[R60] 只看 HTTP 状态码
来源：http://anv.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jif.ydjk.org.cn

[R61] 磁盘占用
来源：http://nhl.guowangkeji.top

df -h;  du -sh *
来源：http://rmn.vqdsnc.cn

[R62] 找最占空间的文件
来源：http://rkn.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://qmu.xuetiantiany.cn

[R63] 内存与进程
来源：http://uni.ctjpmb.com

free -h;  ps aux | grep nginx
来源：http://qny.epnwcf.com

[R64] 结束进程
来源：http://ehl.yfazqb.com

kill -9 $(pgrep -f app.py)
来源：http://xqu.uphjek.com

[R65] 查看端口占用
来源：http://qbm.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cxu.hesvh.cn

[R66] 定时任务
来源：http://dkg.jinyuanbaomall.cn

crontab -e;  crontab -l
来源：http://xhg.hcnkem.com

[R67] 生成随机十六进制串
来源：http://wem.hesvh.cn

openssl rand -hex 16
来源：http://mju.xziqi.cn

[R68] 计算文件校验值
来源：http://mdq.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pqx.epnwcf.com

[R69] 生成随机密码
来源：http://fit.aibaodan.cn

head -c 16 /dev/urandom | base64
来源：http://biz.shuidangran.top

[R70] 时间戳与互转
来源：http://jhj.yfazqb.com

date +%s;  date -d @1700000000
来源：http://kkm.svipenyu.cn

[R71] 日期格式化
来源：http://pfb.guowangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://aoi.mhx1999.top

[R72] 等待端口就绪
来源：http://zqj.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tlb.fzhhl.top

[R73] 分割大日志
来源：http://xbk.jlsjyb.cn

split -l 1000 big.log part_
来源：http://ruh.jlsjyb.cn

[R74] 批量重命名
来源：http://vzj.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bmi.zdqjudy.top

[R75] 导出环境变量
来源：http://uoa.cucudq.cn

export PATH="$HOME/bin:$PATH"
来源：http://fkz.guowangkeji.top

[R76] 使用临时文件
来源：http://nnv.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bhb.hongshengwenyu.top

[R77] 读取用户输入
来源：http://hdl.gzhubu.top

read -rp "请输入: " ans
来源：http://jur.ybcxt.top

[R78] 交互式菜单
来源：http://jwn.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wib.sxryk.cn

[R79] 解析命令行选项
来源：http://nlt.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://abt.vehdjk.com

[R80] 查看脚本执行耗时
来源：http://hjd.havefunace.top

time ./run.sh
来源：http://jpg.yangfankeji.com

================================================================================
来源：http://tdw.ydjk.org.cn

S. C / C++ 专题
来源：http://gzh.cdnleiting.top

================================================================================
来源：http://puk.cdnleiting.top

[S01] C：Hello World
来源：http://twp.epnwcf.com

#include <stdio.h>
来源：http://jwh.daxiang520.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://bmh.yj20258888.top

[S02] C：变量与格式化输出
来源：http://tgg.fktsv.cn

int a = 10; printf("%d\n", a);
来源：http://geg.cqqwz.cn

[S03] C：读入整数
来源：http://sog.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://yhi.ywan-chungtsiang.top

[S04] C：字符串复制
来源：http://ezr.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://ive.ywan-chungtsiang.top

[S05] C：字符串长度
来源：http://bsp.chenzaomai.com

strlen(s)
来源：http://wnn.yueranfly.top

[S06] C：字符串比较
来源：http://kzs.meibo888.top

strcmp(a, b) == 0
来源：http://jfk.fktsv.cn

[S07] C：数组遍历求和
来源：http://jtn.fehbvm.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tiq.nanxuanxn.top

[S08] C：动态内存分配与释放
来源：http://rrd.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rox.yj20258.top

[S09] C：结构体定义与初始化
来源：http://rwc.vqdsnc.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wlk.gotoacloud.top

[S10] C：指针与解引用
来源：http://kks.epnwcf.com

int *p = &a;  *p = 5;
来源：http://sla.zhongyouzk.top

[S11] C：逐行读文件
来源：http://aiv.yonumen.top

FILE *f = fopen("a.txt", "r");
来源：http://mwe.xylfe.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mzx.wangdashe.top

fclose(f);
来源：http://sro.gotoacloud.top

[S12] C：写文件
来源：http://brp.guannengcc.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vwe.xziqi.cn

[S13] C：宏定义
来源：http://uot.guannengcc.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qnf.dashuyun.cn

[S14] C：枚举
来源：http://daw.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://pbv.chenzaomai.com

[S15] C：类型转换
来源：http://ioe.yueranfly.top

(double) a / b
来源：http://dbc.wangdashe.top

[S16] C：位操作置位
来源：http://sla.nwbrower.top

x |= (1 << 3);
来源：http://cbc.quarkkingdee.top

[S17] C：安全拼接字符串
来源：http://zzw.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://alw.tian-w.cn

[S18] C：命令行参数
来源：http://axq.shuidangran.top

int main(int argc, char **argv)
来源：http://exy.zhengqikj.top

[S19] C：快速排序
来源：http://hhw.jyoumei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rgh.gzhubu.top

[S20] C：二分查找
来源：http://kbf.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kjx.zhengqikj.top

[S21] C：字符类别判断
来源：http://ajf.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dyc.jinqigfzy.top

[S22] C：字符串转数字
来源：http://esk.ehwqpu.com

atoi("42");  strtod("3.14", NULL);
来源：http://mbw.zhijiandao.cn

[S23] C：随机数
来源：http://jgj.hnxiangtu.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hcv.sweek.top

[S24] C：获取本地时间
来源：http://oda.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://soh.316326.xyz

[S25] C：内存拷贝
来源：http://kuc.ctjpmb.com

memcpy(dst, src, n);
来源：http://gjb.ivvv.top

[S26] C：内存清零
来源：http://mxo.fktsv.cn

memset(a, 0, sizeof a);
来源：http://sxv.yvedp.cn

[S27] C：定义常量
来源：http://uca.zycfv.cn

const double PI = 3.14159;
来源：http://eae.yangfankeji.com

[S28] C：静态变量
来源：http://pxl.yfazqb.com

static int counter = 0;
来源：http://uki.yvedp.cn

[S29] C：变参函数
来源：http://lgi.yuanzhike.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://enu.hnxiangtu.top

[S30] C：头文件保护
来源：http://zff.fanxiaobao.xyz

#ifndef X_H
来源：http://jfe.vehdjk.com

#define X_H
来源：http://qll.chenlongwang.top

#endif
来源：http://hvh.cdnleiting.top

[S31] C++：Hello World
来源：http://oev.dashuyun.cn

#include <iostream>
来源：http://kpd.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://yvc.hcnkem.com

[S32] C++：字符串
来源：http://eau.guowangkeji.top

std::string s = "hi";  s += "!";
来源：http://nro.yj20258888.top

[S33] C++：vector 增删
来源：http://wed.chenzaomai.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wfh.birdmap.top

[S34] C++：遍历 vector
来源：http://skk.ctjpmb.com

for (auto &x : v) { std::cout << x; }
来源：http://duf.yuanzhike.top

[S35] C++：map
来源：http://ghc.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xer.yuanzhike.top

[S36] C++：unordered_map
来源：http://mku.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wcy.dashuyun.cn

[S37] C++：set
来源：http://vnm.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jnx.feifeiyinyue.top

[S38] C++：排序
来源：http://huy.smart0.xyz

std::sort(v.begin(), v.end());
来源：http://poz.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://cxv.mhx1999.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fzv.xuetiantiany.cn

[S40] C++：查找元素
来源：http://pcq.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kdu.gotoacloud.top

[S41] C++：类与构造函数
来源：http://ade.wangshuangyany.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vxf.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://tdd.smart0.xyz

class B : public Base { public: void f() override {} };
来源：http://ojh.316326.xyz

[S43] C++：智能指针
来源：http://zre.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://vbl.jqgfzy.top

[S44] C++：引用传参
来源：http://tkd.zhengqikj.top

void inc(int &x) { ++x; }
来源：http://slx.zdqjudy.top

[S45] C++：lambda
来源：http://xhm.cdnleiting.top

auto add = [](int a, int b) { return a + b; };
来源：http://ypn.zhoulong.xyz

[S46] C++：函数模板
来源：http://hwt.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://znh.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://uwu.havefunace.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bci.hcnkem.com

[S48] C++：逐行读文件
来源：http://fuc.yj20258.top

std::ifstream in("a.txt");  std::string line;
来源：http://xcl.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://swb.guannengcc.top

[S49] C++：写文件
来源：http://qib.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wxv.wangdashe.top

[S50] C++：格式化数字
来源：http://jts.havefunace.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cxb.daria6918.cn

[S51] C++：显式类型转换
来源：http://ueh.hfpthk.cn

static_cast<double>(a) / b
来源：http://ifs.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://kpx.cashguo.top

int size() const noexcept { return n_; }
来源：http://jiq.shanyushiyangtech.top

[S53] C++：移动语义
来源：http://kqr.jlsjyb.cn

std::vector<int> w = std::move(v);
来源：http://uqq.redwolf501.top

[S54] C++：异常处理
来源：http://djk.aibaodan.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ido.vqdsnc.cn

[S55] C++：结构化绑定
来源：http://akl.sjlbkw.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gho.jianghu66.top

[S56] C++：optional
来源：http://mbi.jiagoushi.top


<!-- 参考信息 -->