代发 wailian999

[Q82] 字符长度与字节长度
来源：http://tya.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://gbp.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://qnz.zhiwuduotai.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://foc.ybcxt.top

[Q84] 去除首尾空格
来源：http://mpb.andypj.xyz

SELECT TRIM(name) FROM users;
来源：http://brf.c1oappe.top

[Q85] 数值取整
来源：http://lnc.fzhhl.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bkh.hfpthk.cn

[Q86] 读取 JSON 字段
来源：http://exr.hywenlv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rbu.shangyingyoupin.top

[Q87] JSON 字段做条件
来源：http://xrq.guowangkeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ruh.haohaochexian.top

[Q88] 行转列（条件聚合）
来源：http://zov.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ahb.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xad.sweek.top

[Q89] 判断表是否存在
来源：http://rqu.nwbrower.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ktn.xingfuxueyuan.xyz

[Q90] 生成序号列
来源：http://wsd.pengpengdd.cyou

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://aat.svipenyu.cn

================================================================================
来源：http://blz.tianlin.xyz

R. Bash 专题
来源：http://toy.jianghu66.top

================================================================================
来源：http://uvk.quarkkingdee.top

[R01] shebang 与严格模式
来源：http://sgx.fanxiaobao.xyz

#!/usr/bin/env bash
来源：http://izr.yj202588.top

set -euo pipefail
来源：http://dym.wangdashe.top

[R02] 变量赋值与使用
来源：http://cnk.gogol.net.cn

name="Tom"; echo "$name"
来源：http://jgv.smart0.xyz

[R03] 只读变量
来源：http://qwr.yongpay.top

readonly PI=3.14
来源：http://vcs.ybcxt.top

[R04] 位置参数
来源：http://cqs.nanxuanxn.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vsd.kuanghao11.cn

[R05] 参数默认值
来源：http://erd.xylfe.cn

name="${1:-default}"
来源：http://qsa.guowangkeji.top

[R06] 判断命令是否存在
来源：http://ogo.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ngf.nanxuanxn.top

[R07] if 判断文件
来源：http://jkl.nwbrower.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://zhq.shuidangran.top

[R08] 数值比较
来源：http://nuh.zhongyouzk.top

if (( a > b )); then echo "a 更大"; fi
来源：http://nnx.fanxiaobao.xyz

[R09] 字符串比较
来源：http://git.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zir.jiagoushi.top

[R10] 正则匹配
来源：http://mcs.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ait.snrcjt.cn

[R11] case 多分支
来源：http://oof.tianlin.xyz

case "$1" in
来源：http://rbw.c1oappe.top

start) echo "启动" ;;
来源：http://fjm.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://ywc.xuanzx.com

*)     echo "未知命令" ;;
来源：http://glo.shzxlz.cn

esac
来源：http://psu.hesvh.cn

[R12] for 遍历文件
来源：http://ifs.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://qzf.zhijiandao.cn

[R13] for 计数循环
来源：http://uxw.birdmap.top

for i in {1..10}; do echo "$i"; done
来源：http://jow.guannengcc.top

[R14] C 风格 for
来源：http://fjm.smart0.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nni.yfazqb.com

[R15] while 逐行读文件
来源：http://kax.jinqigufen.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wji.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://xvm.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vpd.0kj1m.cn

[R17] 数组定义与取值
来源：http://kxe.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vcn.c1oappe.top

[R18] 遍历数组
来源：http://kcm.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pby.hfpthk.cn

[R19] 数组长度
来源：http://sel.bbcook.cn

echo "${#arr[@]}"
来源：http://xzm.xuanzx.com

[R20] 关联数组（字典）
来源：http://yuh.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ksp.wangshuangyany.cn

[R21] 字符串长度
来源：http://nhn.sweek.top

echo "${#s}"
来源：http://hfg.gotoacloud.top

[R22] 截取子串
来源：http://yvd.shanyushiyangtech.top

echo "${s:0:5}"
来源：http://gyc.dashuyun.cn

[R23] 字符串替换
来源：http://uhh.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rvr.zhijiandao.cn

[R24] 大小写转换
来源：http://zjk.jinqigfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://sdf.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://svd.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://peg.jinghuilouyu.cn

[R26] 命令替换
来源：http://vpt.fengsongda.top

now=$(date +%F); echo "$now"
来源：http://szp.jianghu66.top

[R27] 算术展开
来源：http://bxo.yangfankeji.com

echo $((1 + 2 * 3))
来源：http://qwm.sxryk.cn

[R28] 浮点运算
来源：http://hsc.guowangkeji.top

echo "scale=2; 10/3" | bc
来源：http://imh.yanxiufei.cn

[R29] 定义函数
来源：http://aac.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qmu.bbcook.cn

[R30] 函数返回状态码
来源：http://vkz.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://szo.epnwcf.com

[R31] 局部变量
来源：http://kid.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://vcg.zhongyouzk.top

[R32] 参数个数校验
来源：http://oap.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lrc.gzhubu.top

[R33] 捕获错误并提示行号
来源：http://ntd.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cqb.cucudq.cn

[R34] 退出时清理
来源：http://jsi.hcnkem.com

trap 'rm -f "$tmp"' EXIT
来源：http://dyv.9152youxi.cn

[R35] 后台执行并等待
来源：http://asp.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ebx.redwolf501.top

[R36] 并发执行多个任务
来源：http://pir.yanxiufei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lpg.9152youxi.cn

[R37] 把输出赋给变量
来源：http://nwa.iojbl.cn

files=$(ls -1)
来源：http://jsv.yanxiufei.cn

[R38] 管道串联
来源：http://nqt.shangyingyoupin.top

cat a.txt | grep -i error | wc -l
来源：http://uac.yuanzhike.top

[R39] 重定向标准输出与错误
来源：http://ctu.zhoulong.xyz

cmd > out.log 2>&1
来源：http://lph.redwolf501.top

[R40] 追加写日志
来源：http://auc.zhixingplan.top

echo "log" >> out.log
来源：http://ear.ivvv.top

[R41] 丢弃输出
来源：http://irk.hcnkem.com

cmd >/dev/null 2>&1
来源：http://gch.jinqigfzy.top

[R42] 输入重定向
来源：http://xmf.shangyingyoupin.top

wc -l < a.txt
来源：http://trl.jiagoushi.top

[R43] 按名字查找文件
来源：http://aft.gaohongyu789.top

find . -name "*.log" -type f
来源：http://tye.ehwqpu.com

[R44] 按修改时间查找
来源：http://rpa.yj20258888.top

find . -mtime -7 -type f
来源：http://vyl.fktsv.cn

[R45] 批量删除
来源：http://unh.xziqi.cn

find . -name "*.tmp" -delete
来源：http://nkt.nanxinkj.top

[R46] 递归替换文件内容
来源：http://ghl.jinqigufen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wwz.zdbjq.cn

[R47] sed 单行替换
来源：http://vka.guannengcc.top

sed -i 's/foo/bar/g' a.txt
来源：http://vzb.ivvv.top

[R48] awk 取指定列
来源：http://jgm.hnxiangtu.top

awk '{print $1, $3}' a.txt
来源：http://icy.cdnleiting.top

[R49] awk 带条件
来源：http://pgs.0kj1m.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://iiw.nanxuanxn.top

[R50] awk 求和
来源：http://mzt.bbcook.cn

awk '{s += $2} END {print s}' a.txt
来源：http://plf.snrcjt.cn

[R51] 排序去重取前几
来源：http://wnr.jinqigufen.top

sort a.txt | uniq -c | sort -rn | head
来源：http://knb.chenjidiqi.icu

[R52] 统计行数
来源：http://ort.hnxiangtu.top

wc -l a.txt
来源：http://kji.ppjwa.cn

[R53] 查看文件头与实时尾
来源：http://oya.yongpay.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dgw.chenlongwang.top

[R54] 比较两个文件
来源：http://cvf.quarkkingdee.top

diff a.txt b.txt
来源：http://djp.sjlbkw.cn

[R55] 压缩与解压
来源：http://zqf.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jir.redwolf501.top

[R56] 远程拷贝
来源：http://ava.ydzc1.top

scp file user@host:/path/
来源：http://jyn.c1oappe.top

[R57] 远程执行命令
来源：http://mjv.birdmap.top

ssh user@host 'uptime'
来源：http://hob.xylfe.cn

[R58] 下载文件
来源：http://fcm.bjfxy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lzd.nanxinkj.top

[R59] 发 POST JSON
来源：http://ymy.chenlongwang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vvw.zhiwuduotai.top

[R60] 只看 HTTP 状态码
来源：http://gea.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://opg.jqgufenzy.top

[R61] 磁盘占用
来源：http://zol.tarul.cn

df -h;  du -sh *
来源：http://qrv.xuanzx.com

[R62] 找最占空间的文件
来源：http://wox.zhiwuduotai.top

du -ah . | sort -rh | head -10
来源：http://cqd.hywenlv.cn

[R63] 内存与进程
来源：http://jrh.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://oyi.aizwys.cn

[R64] 结束进程
来源：http://vfh.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://nai.gzhubu.top

[R65] 查看端口占用
来源：http://sbi.yj202588.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pos.hnqzz.top

[R66] 定时任务
来源：http://jvk.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://uyo.xziqi.cn

[R67] 生成随机十六进制串
来源：http://yko.tianlin.xyz

openssl rand -hex 16
来源：http://wgs.aizwys.cn

[R68] 计算文件校验值
来源：http://wpn.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://wli.smart0.xyz

[R69] 生成随机密码
来源：http://jeu.iojbl.cn

head -c 16 /dev/urandom | base64
来源：http://iee.sxryk.cn

[R70] 时间戳与互转
来源：http://bny.xuanzx.com

date +%s;  date -d @1700000000
来源：http://jha.hywenlv.cn

[R71] 日期格式化
来源：http://cso.aizwys.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvc.fktsv.cn

[R72] 等待端口就绪
来源：http://wat.pycfn.com

until nc -z localhost 3306; do sleep 1; done
来源：http://uqr.epnwcf.com

[R73] 分割大日志
来源：http://xpo.daria6918.cn

split -l 1000 big.log part_
来源：http://fsm.nwbrower.top

[R74] 批量重命名
来源：http://lxn.jiagoushi.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pri.hywenlv.cn

[R75] 导出环境变量
来源：http://yrm.zhaomingkeji.xyz

export PATH="$HOME/bin:$PATH"
来源：http://tnj.jqgfzy.top

[R76] 使用临时文件
来源：http://smt.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rwm.0kj1m.cn

[R77] 读取用户输入
来源：http://kvn.jiagoushi.top

read -rp "请输入: " ans
来源：http://ldy.zhijiandao.cn

[R78] 交互式菜单
来源：http://itw.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://jai.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://hsb.316326.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qsn.kuanghao11.cn

[R80] 查看脚本执行耗时
来源：http://suc.smart0.xyz

time ./run.sh
来源：http://ykf.iojbl.cn

================================================================================
来源：http://yfu.quarkkingdee.top

S. C / C++ 专题
来源：http://tvj.xziqi.cn

================================================================================
来源：http://lqu.fehbvm.com

[S01] C：Hello World
来源：http://mgh.tianlin.xyz

#include <stdio.h>
来源：http://nlt.bjfxy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://sdz.guannengcc.top

[S02] C：变量与格式化输出
来源：http://jti.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://bpe.fengsongda.top

[S03] C：读入整数
来源：http://nwu.yongpay.top

int x; scanf("%d", &x);
来源：http://gdd.nanxinkj.top

[S04] C：字符串复制
来源：http://qlo.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://dft.bbcook.cn

[S05] C：字符串长度
来源：http://gga.xziqi.cn

strlen(s)
来源：http://xer.fktsv.cn

[S06] C：字符串比较
来源：http://lnx.yangfankeji.com

strcmp(a, b) == 0
来源：http://ssz.gotoacloud.top

[S07] C：数组遍历求和
来源：http://sfy.pycfn.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kob.jinqigfzy.top

[S08] C：动态内存分配与释放
来源：http://xhi.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mwb.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://nyy.bbcook.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ojv.quarkkingdee.top

[S10] C：指针与解引用
来源：http://qdr.yuxming.cn

int *p = &a;  *p = 5;
来源：http://web.jqgfzy.top

[S11] C：逐行读文件
来源：http://bdt.tanke756.top

FILE *f = fopen("a.txt", "r");
来源：http://kvr.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://igw.dianchejie.cn

fclose(f);
来源：http://riy.chenlongwang.top

[S12] C：写文件
来源：http://grv.wangdashe.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://grq.cashguo.top

[S13] C：宏定义
来源：http://szl.pengpengdd.cyou

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vmn.hnqzz.top

[S14] C：枚举
来源：http://wgt.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://uwp.vehdjk.com

[S15] C：类型转换
来源：http://eun.hammf.cn

(double) a / b
来源：http://gua.ivvv.top

[S16] C：位操作置位
来源：http://bqt.9152youxi.cn

x |= (1 << 3);
来源：http://kjz.redwolf501.top

[S17] C：安全拼接字符串
来源：http://sox.ctjpmb.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://grf.smart0.xyz

[S18] C：命令行参数
来源：http://lht.zdqjudy.top

int main(int argc, char **argv)
来源：http://ftr.tanke756.top

[S19] C：快速排序
来源：http://zbv.ivvv.top

qsort(a, n, sizeof(int), cmp);
来源：http://smf.guannengcc.top

[S20] C：二分查找
来源：http://zpq.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jtn.316326.xyz

[S21] C：字符类别判断
来源：http://dsp.jinyuanbaomall.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uow.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://vrl.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tzk.ydzc1.top

[S23] C：随机数
来源：http://hxu.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wip.aibaodan.cn

[S24] C：获取本地时间
来源：http://kjt.quarkkingdee.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://idi.yueranfly.top

[S25] C：内存拷贝
来源：http://clg.birdmap.top

memcpy(dst, src, n);
来源：http://azl.tarul.cn

[S26] C：内存清零
来源：http://rtd.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://mkt.wangshuangyany.cn

[S27] C：定义常量
来源：http://ccn.jqgufenzy.top

const double PI = 3.14159;
来源：http://zpi.vqdsnc.cn

[S28] C：静态变量
来源：http://jvp.jinqigufen.top

static int counter = 0;
来源：http://jrb.kuanghao11.cn

[S29] C：变参函数
来源：http://mcc.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ytp.haohaochexian.top

[S30] C：头文件保护
来源：http://cvk.cqqwz.cn

#ifndef X_H
来源：http://mri.chenlongwang.top

#define X_H
来源：http://bch.hnxiangtu.top

#endif
来源：http://zxu.chenjidiqi.icu

[S31] C++：Hello World
来源：http://eje.fzhhl.top

#include <iostream>
来源：http://kbe.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://bhl.cdnleiting.top

[S32] C++：字符串
来源：http://ffw.quarkkingdee.top

std::string s = "hi";  s += "!";
来源：http://mjo.zycfv.cn

[S33] C++：vector 增删
来源：http://fbh.gzhubu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yxu.bjfxy.top

[S34] C++：遍历 vector
来源：http://dmh.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://qst.chenzaomai.com

[S35] C++：map
来源：http://zuj.xylfe.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://amz.jlsjyb.cn

[S36] C++：unordered_map
来源：http://wuo.yuxming.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kbg.fehbvm.com

[S37] C++：set
来源：http://yeo.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gso.redwolf501.top

[S38] C++：排序
来源：http://kpu.zhixingplan.top

std::sort(v.begin(), v.end());
来源：http://cwp.cheryme.top

[S39] C++：自定义比较器排序
来源：http://kye.chenzaomai.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pqu.havefunace.top

[S40] C++：查找元素
来源：http://uvj.chenzaomai.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zdz.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://sqd.havefunace.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pua.hcnkem.com

[S42] C++：继承与虚函数
来源：http://qtc.mhx1999.top

class B : public Base { public: void f() override {} };
来源：http://vkj.cashguo.top

[S43] C++：智能指针
来源：http://fso.zhengqikj.top

auto p = std::make_unique<int>(5);
来源：http://agf.fengsongda.top

[S44] C++：引用传参
来源：http://ykd.cucudq.cn

void inc(int &x) { ++x; }
来源：http://jlv.kuanghao11.cn

[S45] C++：lambda
来源：http://csh.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://rij.yuxming.cn

[S46] C++：函数模板
来源：http://cao.nanxinkj.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vnl.vqdsnc.cn

[S47] C++：结构化绑定遍历
来源：http://bsm.shzxlz.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mjx.yuanzhike.top

[S48] C++：逐行读文件
来源：http://fbl.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://psu.bbcook.cn

while (std::getline(in, line)) { }
来源：http://ncq.hammf.cn

[S49] C++：写文件
来源：http://vgg.wangdashe.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gje.ehwqpu.com

[S50] C++：格式化数字
来源：http://hrg.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://asq.0kj1m.cn

[S51] C++：显式类型转换
来源：http://odx.zhoulong.xyz

static_cast<double>(a) / b
来源：http://wgo.hnxiangtu.top

[S52] C++：const 与 noexcept
来源：http://qhh.yj20258888.top


<!-- 参考信息 -->