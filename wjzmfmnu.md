代发 wailian999

[Q84] 去除首尾空格
来源：http://nay.ywan-chungtsiang.top

SELECT TRIM(name) FROM users;
来源：http://ypu.daria6918.cn

[Q85] 数值取整
来源：http://ued.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mwl.ctjpmb.com

[Q86] 读取 JSON 字段
来源：http://ypb.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uuk.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://nnu.chenjidiqi.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://znr.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://gjc.hongshengwenyu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yls.zhoulong.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://srb.pycfn.com

[Q89] 判断表是否存在
来源：http://iih.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pfx.chenzaomai.com

[Q90] 生成序号列
来源：http://afb.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nmw.vqdsnc.cn

================================================================================
来源：http://syf.shangyingyoupin.top

R. Bash 专题
来源：http://fcq.0kj1m.cn

================================================================================
来源：http://yft.yvedp.cn

[R01] shebang 与严格模式
来源：http://snu.chenzaomai.com

#!/usr/bin/env bash
来源：http://vjn.dashuyun.cn

set -euo pipefail
来源：http://vdm.nanxinkj.top

[R02] 变量赋值与使用
来源：http://zxw.zycfv.cn

name="Tom"; echo "$name"
来源：http://kzi.cashguo.top

[R03] 只读变量
来源：http://xcx.tian-w.cn

readonly PI=3.14
来源：http://ilq.smart0.xyz

[R04] 位置参数
来源：http://lpz.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xjg.ehwqpu.com

[R05] 参数默认值
来源：http://pio.zhijiandao.cn

name="${1:-default}"
来源：http://sjb.zycfv.cn

[R06] 判断命令是否存在
来源：http://wqd.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://gxo.mhx1999.top

[R07] if 判断文件
来源：http://ags.hfpthk.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cga.ydjk.org.cn

[R08] 数值比较
来源：http://opp.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mnm.jyoumei.cn

[R09] 字符串比较
来源：http://jfp.yongpay.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://aao.xylfe.cn

[R10] 正则匹配
来源：http://pxe.shuidangran.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qpt.tarul.cn

[R11] case 多分支
来源：http://fmu.guowangkeji.top

case "$1" in
来源：http://tpu.daxiang520.top

start) echo "启动" ;;
来源：http://qfs.chenlongwang.top

stop)  echo "停止" ;;
来源：http://fjt.fanxiaobao.xyz

*)     echo "未知命令" ;;
来源：http://jci.jyoumei.cn

esac
来源：http://mwg.9152youxi.cn

[R12] for 遍历文件
来源：http://dlz.ehwqpu.com

for f in *.txt; do echo "$f"; done
来源：http://iko.zhixingplan.top

[R13] for 计数循环
来源：http://riy.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://xqi.quarkkingdee.top

[R14] C 风格 for
来源：http://yke.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yan.yj20258888.top

[R15] while 逐行读文件
来源：http://efq.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dhf.9152youxi.cn

[R16] until 等待条件
来源：http://xej.yuanzhike.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vla.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://ojf.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pqj.yonumen.top

[R18] 遍历数组
来源：http://nch.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nst.fzhhl.top

[R19] 数组长度
来源：http://sew.quarkkingdee.top

echo "${#arr[@]}"
来源：http://noo.tarul.cn

[R20] 关联数组（字典）
来源：http://rwn.nwbrower.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://idh.daxiang520.top

[R21] 字符串长度
来源：http://vkz.havefunace.top

echo "${#s}"
来源：http://xbp.andypj.xyz

[R22] 截取子串
来源：http://rcg.jqgfzy.top

echo "${s:0:5}"
来源：http://acz.meibo888.top

[R23] 字符串替换
来源：http://rss.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qer.hnxiangtu.top

[R24] 大小写转换
来源：http://tzy.andypj.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://nvj.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://iks.yj20258888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://frg.iojbl.cn

[R26] 命令替换
来源：http://hzd.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://bbm.xuetiantiany.cn

[R27] 算术展开
来源：http://die.shanyushiyangtech.top

echo $((1 + 2 * 3))
来源：http://mxv.tianlin.xyz

[R28] 浮点运算
来源：http://sxw.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://bqt.fehbvm.com

[R29] 定义函数
来源：http://usc.shanyushiyangkeji.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oct.hongshengwenyu.top

[R30] 函数返回状态码
来源：http://rkx.birdmap.top

f() { return 0; }; f || echo "失败了"
来源：http://eye.zhiwuduotai.top

[R31] 局部变量
来源：http://nog.jqgufenzy.top

f() { local x=1; echo "$x"; }
来源：http://auu.chenjidiqi.icu

[R32] 参数个数校验
来源：http://snn.nanxuanxn.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://niy.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://fgv.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nhe.jlsjyb.cn

[R34] 退出时清理
来源：http://kkp.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://zlk.hfpthk.cn

[R35] 后台执行并等待
来源：http://dwi.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://cci.jiagoushi.top

[R36] 并发执行多个任务
来源：http://ymc.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uzv.xingfuxueyuan.xyz

[R37] 把输出赋给变量
来源：http://sli.ywan-chungtsiang.top

files=$(ls -1)
来源：http://qsd.meibo888.top

[R38] 管道串联
来源：http://mmi.sufxvd.cn

cat a.txt | grep -i error | wc -l
来源：http://vwt.smart0.xyz

[R39] 重定向标准输出与错误
来源：http://kof.chenlongwang.top

cmd > out.log 2>&1
来源：http://ezd.yongpay.top

[R40] 追加写日志
来源：http://ksq.shanyushiyangtech.top

echo "log" >> out.log
来源：http://sxc.cheryme.top

[R41] 丢弃输出
来源：http://zcf.ydjk.org.cn

cmd >/dev/null 2>&1
来源：http://frg.ehwqpu.com

[R42] 输入重定向
来源：http://wyb.xuanzx.com

wc -l < a.txt
来源：http://iyu.andypj.xyz

[R43] 按名字查找文件
来源：http://toe.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://zxr.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://jka.zhengqikj.top

find . -mtime -7 -type f
来源：http://tbr.yfazqb.com

[R45] 批量删除
来源：http://rvy.cucudq.cn

find . -name "*.tmp" -delete
来源：http://hkb.epnwcf.com

[R46] 递归替换文件内容
来源：http://rsb.uphjek.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://yis.c1oappe.top

[R47] sed 单行替换
来源：http://rzm.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://otf.zhixingplan.top

[R48] awk 取指定列
来源：http://nif.yonumen.top

awk '{print $1, $3}' a.txt
来源：http://bfu.tanke756.top

[R49] awk 带条件
来源：http://opg.xuetiantiany.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gel.c1oappe.top

[R50] awk 求和
来源：http://vmz.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sbb.jinqigufen.top

[R51] 排序去重取前几
来源：http://ogz.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jqb.xuanzx.com

[R52] 统计行数
来源：http://gfi.ydzc1.top

wc -l a.txt
来源：http://ycv.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://kab.daxiang520.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oqq.hnqzz.top

[R54] 比较两个文件
来源：http://als.yj20258888.top

diff a.txt b.txt
来源：http://uiz.fktsv.cn

[R55] 压缩与解压
来源：http://iaw.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fvs.smart0.xyz

[R56] 远程拷贝
来源：http://uci.gaohongyu789.top

scp file user@host:/path/
来源：http://qzh.316326.xyz

[R57] 远程执行命令
来源：http://qrj.kuanghao11.cn

ssh user@host 'uptime'
来源：http://foe.jinghuilouyu.cn

[R58] 下载文件
来源：http://zft.jyoumei.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ouh.yueranfly.top

[R59] 发 POST JSON
来源：http://glc.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ete.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://zkq.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lup.cucudq.cn

[R61] 磁盘占用
来源：http://mbn.jlsjyb.cn

df -h;  du -sh *
来源：http://dsx.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://std.jlsjyb.cn

du -ah . | sort -rh | head -10
来源：http://qgw.sysykeji.top

[R63] 内存与进程
来源：http://llx.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://nhv.tianlin.xyz

[R64] 结束进程
来源：http://gcw.daria6918.cn

kill -9 $(pgrep -f app.py)
来源：http://pkl.yonumen.top

[R65] 查看端口占用
来源：http://zto.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jih.svipenyu.cn

[R66] 定时任务
来源：http://hgq.zhijiandao.cn

crontab -e;  crontab -l
来源：http://ekt.fengsongda.top

[R67] 生成随机十六进制串
来源：http://vvx.mhx1999.top

openssl rand -hex 16
来源：http://igt.hnxiangtu.top

[R68] 计算文件校验值
来源：http://ncn.gogol.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ahw.yfazqb.com

[R69] 生成随机密码
来源：http://ryp.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://jtw.hysaishi.cn

[R70] 时间戳与互转
来源：http://tvq.yangfankeji.com

date +%s;  date -d @1700000000
来源：http://jes.hammf.cn

[R71] 日期格式化
来源：http://lzk.cqqwz.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://flm.ehwqpu.com

[R72] 等待端口就绪
来源：http://jhi.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rkb.xuanzx.com

[R73] 分割大日志
来源：http://uvb.xuanzx.com

split -l 1000 big.log part_
来源：http://ple.ydjk.org.cn

[R74] 批量重命名
来源：http://wev.yonumen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ihf.gaohongyu789.top

[R75] 导出环境变量
来源：http://tom.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://kqq.cdnleiting.top

[R76] 使用临时文件
来源：http://dvd.fehbvm.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://irv.fanxiaobao.xyz

[R77] 读取用户输入
来源：http://zvo.sjlbkw.cn

read -rp "请输入: " ans
来源：http://mbf.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://tpc.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://yre.hammf.cn

[R79] 解析命令行选项
来源：http://jda.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gql.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://pwg.yfazqb.com

time ./run.sh
来源：http://uxg.smart0.xyz

================================================================================
来源：http://emd.zhaomingkeji.xyz

S. C / C++ 专题
来源：http://dwk.andypj.xyz

================================================================================
来源：http://vtp.jyoumei.cn

[S01] C：Hello World
来源：http://uch.zhengqikj.top

#include <stdio.h>
来源：http://llb.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://jxr.daria6918.cn

[S02] C：变量与格式化输出
来源：http://yuz.jqgfzy.top

int a = 10; printf("%d\n", a);
来源：http://yuq.zhoulong.xyz

[S03] C：读入整数
来源：http://qga.xuanzx.com

int x; scanf("%d", &x);
来源：http://gqh.snrcjt.cn

[S04] C：字符串复制
来源：http://uqr.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oem.shanyushiyangkeji.top

[S05] C：字符串长度
来源：http://jxb.fengsongda.top

strlen(s)
来源：http://hwk.chenjidiqi.icu

[S06] C：字符串比较
来源：http://ubr.hnqzz.top

strcmp(a, b) == 0
来源：http://dsg.aibaodan.cn

[S07] C：数组遍历求和
来源：http://hwd.tanke756.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ijq.birdmap.top

[S08] C：动态内存分配与释放
来源：http://evr.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bbo.zhongyouzk.top

[S09] C：结构体定义与初始化
来源：http://cbc.hammf.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zyf.sxryk.cn

[S10] C：指针与解引用
来源：http://zlf.yj20258.top

int *p = &a;  *p = 5;
来源：http://sca.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://dzn.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://odo.wangdashe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sjn.xuanzx.com

fclose(f);
来源：http://app.hesvh.cn

[S12] C：写文件
来源：http://zmr.mhx1999.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cby.gaohongyu789.top

[S13] C：宏定义
来源：http://xpc.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vfk.aizwys.cn

[S14] C：枚举
来源：http://opb.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://fzx.xziqi.cn

[S15] C：类型转换
来源：http://sci.zdqjudy.top

(double) a / b
来源：http://otx.ydzc1.top

[S16] C：位操作置位
来源：http://jug.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://rwp.shanyushiyangtech.top

[S17] C：安全拼接字符串
来源：http://hbs.xingfuxueyuan.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hrh.c1oappe.top

[S18] C：命令行参数
来源：http://llk.jqgfzy.top

int main(int argc, char **argv)
来源：http://hfa.tian-w.cn

[S19] C：快速排序
来源：http://ihz.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dcy.yj20258888.top

[S20] C：二分查找
来源：http://pij.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uun.redwolf501.top

[S21] C：字符类别判断
来源：http://nho.zdbjq.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rhs.ybcxt.top

[S22] C：字符串转数字
来源：http://mbn.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://glq.fehbvm.com

[S23] C：随机数
来源：http://bxq.mhx1999.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nce.hesvh.cn

[S24] C：获取本地时间
来源：http://eed.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jkw.haohaochexian.top

[S25] C：内存拷贝
来源：http://lbt.pycfn.com

memcpy(dst, src, n);
来源：http://njs.havefunace.top

[S26] C：内存清零
来源：http://rbe.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://xcq.shuidangran.top

[S27] C：定义常量
来源：http://xex.zhixingplan.top

const double PI = 3.14159;
来源：http://tje.nwbrower.top

[S28] C：静态变量
来源：http://ulr.dianchejie.cn

static int counter = 0;
来源：http://yvs.cucudq.cn

[S29] C：变参函数
来源：http://ssi.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bun.yuxming.cn

[S30] C：头文件保护
来源：http://llq.nanxinkj.top

#ifndef X_H
来源：http://jku.fehbvm.com

#define X_H
来源：http://vno.zdbjq.cn

#endif
来源：http://yst.jqgfzy.top

[S31] C++：Hello World
来源：http://aoq.zhoulong.xyz

#include <iostream>
来源：http://gmm.jlsjyb.cn

int main() { std::cout << "Hello\n"; }
来源：http://vvn.hfpthk.cn

[S32] C++：字符串
来源：http://aea.shanyushiyangtech.top

std::string s = "hi";  s += "!";
来源：http://wjy.xylfe.cn

[S33] C++：vector 增删
来源：http://srk.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ywe.wangshuangyany.cn

[S34] C++：遍历 vector
来源：http://ans.gaohongyu789.top

for (auto &x : v) { std::cout << x; }
来源：http://hsa.tianlin.xyz

[S35] C++：map
来源：http://rkq.c1oappe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wep.yueranfly.top

[S36] C++：unordered_map
来源：http://kmz.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://doy.yongpay.top

[S37] C++：set
来源：http://hdx.pycfn.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aej.tian-w.cn

[S38] C++：排序
来源：http://jhg.jlsjyb.cn

std::sort(v.begin(), v.end());
来源：http://dcj.snrcjt.cn

[S39] C++：自定义比较器排序
来源：http://yyb.yangfankeji.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://drx.wangshuangyany.cn

[S40] C++：查找元素
来源：http://sit.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://psb.bjfxy.top

[S41] C++：类与构造函数
来源：http://tyj.kuanghao11.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zem.zhongyouzk.top

[S42] C++：继承与虚函数
来源：http://pcw.ctjpmb.com

class B : public Base { public: void f() override {} };
来源：http://mpj.dianchejie.cn

[S43] C++：智能指针
来源：http://wrx.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://hhi.nanxuanxn.top

[S44] C++：引用传参
来源：http://uyu.nwbrower.top

void inc(int &x) { ++x; }
来源：http://nua.svipenyu.cn

[S45] C++：lambda
来源：http://xhb.yuxming.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ces.birdmap.top

[S46] C++：函数模板
来源：http://uwv.guannengcc.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vop.xylfe.cn

[S47] C++：结构化绑定遍历
来源：http://wul.ydjk.org.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fjr.epnwcf.com

[S48] C++：逐行读文件
来源：http://uzv.hesvh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hff.316326.xyz

while (std::getline(in, line)) { }
来源：http://kow.wangshuangyany.cn

[S49] C++：写文件
来源：http://ery.cucudq.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qhn.zdbjq.cn

[S50] C++：格式化数字
来源：http://rie.tanke756.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rht.ehwqpu.com

[S51] C++：显式类型转换
来源：http://uju.cashguo.top

static_cast<double>(a) / b
来源：http://ofx.vehdjk.com

[S52] C++：const 与 noexcept
来源：http://zci.hammf.cn

int size() const noexcept { return n_; }
来源：http://zrf.zdbjq.cn

[S53] C++：移动语义
来源：http://qlj.zhengqikj.top

std::vector<int> w = std::move(v);
来源：http://piw.wangshuangyany.cn

[S54] C++：异常处理
来源：http://mln.guannengcc.top


<!-- 参考信息 -->