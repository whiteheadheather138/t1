代发 wailian999

[Q84] 去除首尾空格
来源：http://tfh.jinqigfzy.top

SELECT TRIM(name) FROM users;
来源：http://pou.sxryk.cn

[Q85] 数值取整
来源：http://vvs.fehbvm.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ljt.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://fou.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gza.yongpay.top

[Q87] JSON 字段做条件
来源：http://jrx.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xvw.jqgfzy.top

[Q88] 行转列（条件聚合）
来源：http://egd.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://lgh.hnqzz.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://jjy.hammf.cn

[Q89] 判断表是否存在
来源：http://nrw.gaohongyu789.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ddp.wangdashe.top

[Q90] 生成序号列
来源：http://vhl.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wlz.dashuyun.cn

================================================================================
来源：http://qaw.zhijiandao.cn

R. Bash 专题
来源：http://nem.epnwcf.com

================================================================================
来源：http://gxp.guowangkeji.top

[R01] shebang 与严格模式
来源：http://pec.shanyushiyangtech.top

#!/usr/bin/env bash
来源：http://jvj.pengpengdd.cyou

set -euo pipefail
来源：http://dns.sysykeji.top

[R02] 变量赋值与使用
来源：http://eqm.gogol.net.cn

name="Tom"; echo "$name"
来源：http://mxx.jiagoushi.top

[R03] 只读变量
来源：http://cjc.yuanzhike.top

readonly PI=3.14
来源：http://aiu.xziqi.cn

[R04] 位置参数
来源：http://rnx.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nty.zhiwuduotai.top

[R05] 参数默认值
来源：http://zoj.nwbrower.top

name="${1:-default}"
来源：http://hck.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://dht.vqdsnc.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vdr.jianghu66.top

[R07] if 判断文件
来源：http://irz.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eqd.haohaochexian.top

[R08] 数值比较
来源：http://gzr.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nvk.wangshuangyany.cn

[R09] 字符串比较
来源：http://pay.jinqigfzy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oga.xinyue.icu

[R10] 正则匹配
来源：http://lxz.jqgfzy.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ogq.sysykeji.top

[R11] case 多分支
来源：http://gqq.epnwcf.com

case "$1" in
来源：http://rde.hesvh.cn

start) echo "启动" ;;
来源：http://jrt.jyoumei.cn

stop)  echo "停止" ;;
来源：http://dgv.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://kog.gaohongyu789.top

esac
来源：http://pue.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://udx.yonumen.top

for f in *.txt; do echo "$f"; done
来源：http://wxe.hnqzz.top

[R13] for 计数循环
来源：http://rwm.vehdjk.com

for i in {1..10}; do echo "$i"; done
来源：http://grc.yanxiufei.cn

[R14] C 风格 for
来源：http://rnt.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ibv.havefunace.top

[R15] while 逐行读文件
来源：http://ziy.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://whc.aizwys.cn

[R16] until 等待条件
来源：http://kjx.uphjek.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qso.sxryk.cn

[R17] 数组定义与取值
来源：http://pjj.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://yxa.yuxming.cn

[R18] 遍历数组
来源：http://gaq.cheryme.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ria.smart0.xyz

[R19] 数组长度
来源：http://wcp.hnxiangtu.top

echo "${#arr[@]}"
来源：http://qyc.zhijiandao.cn

[R20] 关联数组（字典）
来源：http://mjr.iojbl.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uaz.yongpay.top

[R21] 字符串长度
来源：http://lpw.pycfn.com

echo "${#s}"
来源：http://jeu.haohaochexian.top

[R22] 截取子串
来源：http://epu.hnqzz.top

echo "${s:0:5}"
来源：http://pwh.yongpay.top

[R23] 字符串替换
来源：http://eck.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rrw.ydzc1.top

[R24] 大小写转换
来源：http://upb.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://yfx.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://wum.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://fqk.xinyue.icu

[R26] 命令替换
来源：http://efy.pycfn.com

now=$(date +%F); echo "$now"
来源：http://mhu.yangfankeji.com

[R27] 算术展开
来源：http://mym.tarul.cn

echo $((1 + 2 * 3))
来源：http://nef.birdmap.top

[R28] 浮点运算
来源：http://fyz.zdqjudy.top

echo "scale=2; 10/3" | bc
来源：http://hsd.cdnleiting.top

[R29] 定义函数
来源：http://bga.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://yiy.chenlongwang.top

[R30] 函数返回状态码
来源：http://laz.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://sut.zhijiandao.cn

[R31] 局部变量
来源：http://pdl.yonumen.top

f() { local x=1; echo "$x"; }
来源：http://oqt.redwolf501.top

[R32] 参数个数校验
来源：http://quq.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://kma.fanxiaobao.xyz

[R33] 捕获错误并提示行号
来源：http://agl.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ibx.redwolf501.top

[R34] 退出时清理
来源：http://gid.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://cin.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://kue.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://szx.havefunace.top

[R36] 并发执行多个任务
来源：http://igo.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wwo.jinghuilouyu.cn

[R37] 把输出赋给变量
来源：http://mdf.zhengqikj.top

files=$(ls -1)
来源：http://khy.hywenlv.cn

[R38] 管道串联
来源：http://lmg.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://llb.shuidangran.top

[R39] 重定向标准输出与错误
来源：http://xxo.fzhhl.top

cmd > out.log 2>&1
来源：http://izb.hcnkem.com

[R40] 追加写日志
来源：http://yjk.dianchejie.cn

echo "log" >> out.log
来源：http://zur.gzhubu.top

[R41] 丢弃输出
来源：http://yun.shuidangran.top

cmd >/dev/null 2>&1
来源：http://igl.zhixingplan.top

[R42] 输入重定向
来源：http://xio.zycfv.cn

wc -l < a.txt
来源：http://iil.cdnleiting.top

[R43] 按名字查找文件
来源：http://yaz.hammf.cn

find . -name "*.log" -type f
来源：http://vdw.chenlongwang.top

[R44] 按修改时间查找
来源：http://sbd.tian-w.cn

find . -mtime -7 -type f
来源：http://nxe.wangshuangyany.cn

[R45] 批量删除
来源：http://fyl.pycfn.com

find . -name "*.tmp" -delete
来源：http://ama.hywenlv.cn

[R46] 递归替换文件内容
来源：http://xif.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qjn.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://jsr.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://oyn.yvedp.cn

[R48] awk 取指定列
来源：http://wjs.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://oxc.cashguo.top

[R49] awk 带条件
来源：http://gmg.snrcjt.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ubo.xziqi.cn

[R50] awk 求和
来源：http://ufs.yonumen.top

awk '{s += $2} END {print s}' a.txt
来源：http://vxg.nanxuanxn.top

[R51] 排序去重取前几
来源：http://yfy.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xdk.nwbrower.top

[R52] 统计行数
来源：http://sjw.hnqzz.top

wc -l a.txt
来源：http://xlf.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://fny.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xlq.hcnkem.com

[R54] 比较两个文件
来源：http://usm.bbcook.cn

diff a.txt b.txt
来源：http://hju.sjlbkw.cn

[R55] 压缩与解压
来源：http://nyp.nanxinkj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jro.nwbrower.top

[R56] 远程拷贝
来源：http://huj.cucudq.cn

scp file user@host:/path/
来源：http://tfo.daxiang520.top

[R57] 远程执行命令
来源：http://lsa.ybcxt.top

ssh user@host 'uptime'
来源：http://wiq.sufxvd.cn

[R58] 下载文件
来源：http://wwn.kuanghao11.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bgp.hfpthk.cn

[R59] 发 POST JSON
来源：http://lsh.nanxinkj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rlr.zhaomingkeji.xyz

[R60] 只看 HTTP 状态码
来源：http://rfz.chenzaomai.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://usj.iojbl.cn

[R61] 磁盘占用
来源：http://mfm.sjlbkw.cn

df -h;  du -sh *
来源：http://tqi.hnqzz.top

[R62] 找最占空间的文件
来源：http://qtf.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://sfj.cashguo.top

[R63] 内存与进程
来源：http://hpx.tarul.cn

free -h;  ps aux | grep nginx
来源：http://wtu.jqgfzy.top

[R64] 结束进程
来源：http://ejk.shzxlz.cn

kill -9 $(pgrep -f app.py)
来源：http://pfi.nanxuanxn.top

[R65] 查看端口占用
来源：http://hok.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rpp.9152youxi.cn

[R66] 定时任务
来源：http://krr.zhongyouzk.top

crontab -e;  crontab -l
来源：http://dqu.ydzc1.top

[R67] 生成随机十六进制串
来源：http://qjp.nanxuanxn.top

openssl rand -hex 16
来源：http://grv.shanyushiyangtech.top

[R68] 计算文件校验值
来源：http://blt.nwbrower.top

sha256sum a.txt;  md5sum a.txt
来源：http://orh.hysaishi.cn

[R69] 生成随机密码
来源：http://ykc.fktsv.cn

head -c 16 /dev/urandom | base64
来源：http://kwm.316326.xyz

[R70] 时间戳与互转
来源：http://qoh.havefunace.top

date +%s;  date -d @1700000000
来源：http://yvx.tian-w.cn

[R71] 日期格式化
来源：http://bil.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://usx.zhengqikj.top

[R72] 等待端口就绪
来源：http://yxm.zycfv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fyh.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://khf.fengsongda.top

split -l 1000 big.log part_
来源：http://lok.wangshuangyany.cn

[R74] 批量重命名
来源：http://pvf.yongpay.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://toj.fengsongda.top

[R75] 导出环境变量
来源：http://utf.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://qej.hongshengwenyu.top

[R76] 使用临时文件
来源：http://zhn.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mqi.zhiwuduotai.top

[R77] 读取用户输入
来源：http://bxu.zhengqikj.top

read -rp "请输入: " ans
来源：http://fax.jqgfzy.top

[R78] 交互式菜单
来源：http://dyk.jianghu66.top

select opt in a b c; do echo "$opt"; break; done
来源：http://cqc.xuanzx.com

[R79] 解析命令行选项
来源：http://mtk.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lpc.yfazqb.com

[R80] 查看脚本执行耗时
来源：http://dgc.wangdashe.top

time ./run.sh
来源：http://bpi.shuidangran.top

================================================================================
来源：http://zty.mhx1999.top

S. C / C++ 专题
来源：http://maw.xuetiantiany.cn

================================================================================
来源：http://xjw.zhengqikj.top

[S01] C：Hello World
来源：http://xip.vehdjk.com

#include <stdio.h>
来源：http://xmi.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://oxm.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://evr.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://pfw.tanke756.top

[S03] C：读入整数
来源：http://foq.chenjidiqi.icu

int x; scanf("%d", &x);
来源：http://nhl.hfpthk.cn

[S04] C：字符串复制
来源：http://kir.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zpi.sufxvd.cn

[S05] C：字符串长度
来源：http://vni.zycfv.cn

strlen(s)
来源：http://tkp.yuanzhike.top

[S06] C：字符串比较
来源：http://qcj.jyoumei.cn

strcmp(a, b) == 0
来源：http://yvr.fktsv.cn

[S07] C：数组遍历求和
来源：http://lxr.gogol.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bjz.cheryme.top

[S08] C：动态内存分配与释放
来源：http://kof.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oig.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://yiy.ywan-chungtsiang.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blf.jianghu66.top

[S10] C：指针与解引用
来源：http://tug.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://qlz.guowangkeji.top

[S11] C：逐行读文件
来源：http://hil.daria6918.cn

FILE *f = fopen("a.txt", "r");
来源：http://qki.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yqw.sweek.top

fclose(f);
来源：http://zlx.dianchejie.cn

[S12] C：写文件
来源：http://zve.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wbe.zhongyouzk.top

[S13] C：宏定义
来源：http://kua.jinqigufen.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gqm.kuanghao11.cn

[S14] C：枚举
来源：http://bwe.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://qor.sufxvd.cn

[S15] C：类型转换
来源：http://jgt.9152youxi.cn

(double) a / b
来源：http://vqc.jinqigfzy.top

[S16] C：位操作置位
来源：http://jvh.nanxinkj.top

x |= (1 << 3);
来源：http://djx.vqdsnc.cn

[S17] C：安全拼接字符串
来源：http://dxj.uphjek.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://obw.shuidangran.top

[S18] C：命令行参数
来源：http://igp.xingfuxueyuan.xyz

int main(int argc, char **argv)
来源：http://rjk.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://kfp.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://pbd.wangshuangyany.cn

[S20] C：二分查找
来源：http://pjz.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gut.tanke756.top

[S21] C：字符类别判断
来源：http://mxa.zhixingplan.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hdl.jlsjyb.cn

[S22] C：字符串转数字
来源：http://zaq.fehbvm.com

atoi("42");  strtod("3.14", NULL);
来源：http://bua.zhiwuduotai.top

[S23] C：随机数
来源：http://ydq.gotoacloud.top

srand(time(NULL));  int r = rand() % 100;
来源：http://div.xuanzx.com

[S24] C：获取本地时间
来源：http://nei.guowangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ljc.c1oappe.top

[S25] C：内存拷贝
来源：http://dpx.hnxiangtu.top

memcpy(dst, src, n);
来源：http://xjy.sysykeji.top

[S26] C：内存清零
来源：http://lyb.zhixingplan.top

memset(a, 0, sizeof a);
来源：http://syj.zhiwuduotai.top

[S27] C：定义常量
来源：http://uwf.yfazqb.com

const double PI = 3.14159;
来源：http://jpd.bbcook.cn

[S28] C：静态变量
来源：http://xtl.xziqi.cn

static int counter = 0;
来源：http://zng.9152youxi.cn

[S29] C：变参函数
来源：http://pao.snrcjt.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zvj.jqgufenzy.top

[S30] C：头文件保护
来源：http://con.yvedp.cn

#ifndef X_H
来源：http://xuv.hnxiangtu.top

#define X_H
来源：http://dpz.fengsongda.top

#endif
来源：http://vmz.ybcxt.top

[S31] C++：Hello World
来源：http://agl.gogol.net.cn

#include <iostream>
来源：http://ska.haohaochexian.top

int main() { std::cout << "Hello\n"; }
来源：http://cxw.ctjpmb.com

[S32] C++：字符串
来源：http://tjx.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://llb.c1oappe.top

[S33] C++：vector 增删
来源：http://pep.sweek.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kpc.sweek.top

[S34] C++：遍历 vector
来源：http://zhv.guowangkeji.top

for (auto &x : v) { std::cout << x; }
来源：http://dpw.yj202588.top

[S35] C++：map
来源：http://emw.fengsongda.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xoa.gaohongyu789.top

[S36] C++：unordered_map
来源：http://cwr.meibo888.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sgm.iojbl.cn

[S37] C++：set
来源：http://uaz.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yys.gaohongyu789.top

[S38] C++：排序
来源：http://pge.fehbvm.com

std::sort(v.begin(), v.end());
来源：http://pnm.jyoumei.cn

[S39] C++：自定义比较器排序
来源：http://iqs.cucudq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cpd.chenzaomai.com

[S40] C++：查找元素
来源：http://wzk.svipenyu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fbv.xziqi.cn

[S41] C++：类与构造函数
来源：http://thk.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dwc.cdnleiting.top

[S42] C++：继承与虚函数
来源：http://wwm.jlsjyb.cn

class B : public Base { public: void f() override {} };
来源：http://vqq.zhiwuduotai.top

[S43] C++：智能指针
来源：http://nxi.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://yjd.cashguo.top

[S44] C++：引用传参
来源：http://iue.yonumen.top

void inc(int &x) { ++x; }
来源：http://tgi.svipenyu.cn

[S45] C++：lambda
来源：http://auv.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://fso.daria6918.cn

[S46] C++：函数模板
来源：http://mcr.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ysf.xziqi.cn

[S47] C++：结构化绑定遍历
来源：http://zon.ybcxt.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lco.dianchejie.cn

[S48] C++：逐行读文件
来源：http://bax.jinqigufen.top

std::ifstream in("a.txt");  std::string line;
来源：http://jfu.zhengqikj.top

while (std::getline(in, line)) { }
来源：http://mzk.chenzaomai.com

[S49] C++：写文件
来源：http://zcv.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mhj.chenjidiqi.icu

[S50] C++：格式化数字
来源：http://jsw.hnxiangtu.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xru.ydjk.org.cn

[S51] C++：显式类型转换
来源：http://szj.yj202588.top

static_cast<double>(a) / b
来源：http://nav.yj20258.top

[S52] C++：const 与 noexcept
来源：http://imj.zhijiandao.cn

int size() const noexcept { return n_; }
来源：http://wua.epnwcf.com

[S53] C++：移动语义
来源：http://opx.wangshuangyany.cn

std::vector<int> w = std::move(v);
来源：http://woo.jianghu66.top

[S54] C++：异常处理
来源：http://wds.xylfe.cn


<!-- 参考信息 -->