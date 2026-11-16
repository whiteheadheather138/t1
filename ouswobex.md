代发 wailian999

[Q82] 字符长度与字节长度
来源：http://ttt.havefunace.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ate.daria6918.cn

[Q83] 大小写转换
来源：http://hmd.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://idi.epnwcf.com

[Q84] 去除首尾空格
来源：http://zzk.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://mlo.jinqigfzy.top

[Q85] 数值取整
来源：http://gyh.ivvv.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mll.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://wyv.shzxlz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://let.ydjk.org.cn

[Q87] JSON 字段做条件
来源：http://pxy.yonumen.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xqi.jinqigfzy.top

[Q88] 行转列（条件聚合）
来源：http://nov.chenlongwang.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ugf.yanxiufei.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://onz.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://wcd.zdqjudy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yjy.hammf.cn

[Q90] 生成序号列
来源：http://jyl.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://svs.hywenlv.cn

================================================================================
来源：http://khr.snrcjt.cn

R. Bash 专题
来源：http://ybf.zhengqikj.top

================================================================================
来源：http://zeb.52xcode.cn

[R01] shebang 与严格模式
来源：http://qiv.gzhubu.top

#!/usr/bin/env bash
来源：http://sux.aibaodan.cn

set -euo pipefail
来源：http://ljl.zhengqikj.top

[R02] 变量赋值与使用
来源：http://wic.jinqigufen.top

name="Tom"; echo "$name"
来源：http://cju.xylfe.cn

[R03] 只读变量
来源：http://vji.guowangkeji.top

readonly PI=3.14
来源：http://bwx.gogol.net.cn

[R04] 位置参数
来源：http://ehh.kuanghao11.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ujf.hammf.cn

[R05] 参数默认值
来源：http://lkj.c1oappe.top

name="${1:-default}"
来源：http://pcz.sufxvd.cn

[R06] 判断命令是否存在
来源：http://pli.sufxvd.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xbb.sufxvd.cn

[R07] if 判断文件
来源：http://cwg.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.daxiang520.top

[R08] 数值比较
来源：http://bxq.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tii.cucudq.cn

[R09] 字符串比较
来源：http://lkq.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://oty.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://gie.cucudq.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lmw.redwolf501.top

[R11] case 多分支
来源：http://fqe.cashguo.top

case "$1" in
来源：http://slp.ctjpmb.com

start) echo "启动" ;;
来源：http://ftv.zhongyouzk.top

stop)  echo "停止" ;;
来源：http://rff.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://ery.ehwqpu.com

esac
来源：http://lbl.zdbjq.cn

[R12] for 遍历文件
来源：http://evb.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://mqg.hnxiangtu.top

[R13] for 计数循环
来源：http://hrv.hammf.cn

for i in {1..10}; do echo "$i"; done
来源：http://rng.fzhhl.top

[R14] C 风格 for
来源：http://nai.zhengqikj.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://brj.zhoulong.xyz

[R15] while 逐行读文件
来源：http://rjp.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tzr.hysaishi.cn

[R16] until 等待条件
来源：http://xkh.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yya.sufxvd.cn

[R17] 数组定义与取值
来源：http://zqd.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://kur.ivvv.top

[R18] 遍历数组
来源：http://jlc.wangshuangyany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hny.uphjek.com

[R19] 数组长度
来源：http://wsl.haohaochexian.top

echo "${#arr[@]}"
来源：http://inf.xylfe.cn

[R20] 关联数组（字典）
来源：http://wfg.yfazqb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jqv.fzhhl.top

[R21] 字符串长度
来源：http://cbc.0kj1m.cn

echo "${#s}"
来源：http://inv.yonumen.top

[R22] 截取子串
来源：http://ezp.dianchejie.cn

echo "${s:0:5}"
来源：http://emz.wangdashe.top

[R23] 字符串替换
来源：http://gbq.chenlongwang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iwy.snrcjt.cn

[R24] 大小写转换
来源：http://xdp.9152youxi.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fxl.nwbrower.top

[R25] 去后缀 / 去前缀
来源：http://hbq.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ywy.yj202588.top

[R26] 命令替换
来源：http://whk.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://cba.hfpthk.cn

[R27] 算术展开
来源：http://dye.fzhhl.top

echo $((1 + 2 * 3))
来源：http://zvt.dashuyun.cn

[R28] 浮点运算
来源：http://vck.hysaishi.cn

echo "scale=2; 10/3" | bc
来源：http://gia.bjfxy.top

[R29] 定义函数
来源：http://vgm.xziqi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fna.vehdjk.com

[R30] 函数返回状态码
来源：http://jfp.yanxiufei.cn

f() { return 0; }; f || echo "失败了"
来源：http://uxz.nanxuanxn.top

[R31] 局部变量
来源：http://ryp.cqqwz.cn

f() { local x=1; echo "$x"; }
来源：http://scg.xuanzx.com

[R32] 参数个数校验
来源：http://wie.dianchejie.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://anz.hongshengwenyu.top

[R33] 捕获错误并提示行号
来源：http://soh.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wac.yj202588.top

[R34] 退出时清理
来源：http://uvy.xylfe.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xok.zhengqikj.top

[R35] 后台执行并等待
来源：http://xcv.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jus.yfazqb.com

[R36] 并发执行多个任务
来源：http://vwz.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ntj.daxiang520.top

[R37] 把输出赋给变量
来源：http://qad.zhijiandao.cn

files=$(ls -1)
来源：http://rds.yvedp.cn

[R38] 管道串联
来源：http://vdb.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://wdy.gotoacloud.top

[R39] 重定向标准输出与错误
来源：http://iws.fktsv.cn

cmd > out.log 2>&1
来源：http://qeo.tarul.cn

[R40] 追加写日志
来源：http://voz.yvedp.cn

echo "log" >> out.log
来源：http://bha.dashuyun.cn

[R41] 丢弃输出
来源：http://aoq.cashguo.top

cmd >/dev/null 2>&1
来源：http://edm.jinqigfzy.top

[R42] 输入重定向
来源：http://pjg.havefunace.top

wc -l < a.txt
来源：http://bio.aizwys.cn

[R43] 按名字查找文件
来源：http://sec.yj20258888.top

find . -name "*.log" -type f
来源：http://nas.sysykeji.top

[R44] 按修改时间查找
来源：http://noy.wangdashe.top

find . -mtime -7 -type f
来源：http://ytv.cdnleiting.top

[R45] 批量删除
来源：http://hnj.uphjek.com

find . -name "*.tmp" -delete
来源：http://rci.jyoumei.cn

[R46] 递归替换文件内容
来源：http://tjr.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gdp.yvedp.cn

[R47] sed 单行替换
来源：http://qfy.tianlin.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://wrf.andypj.xyz

[R48] awk 取指定列
来源：http://xnp.shanyushiyangkeji.top

awk '{print $1, $3}' a.txt
来源：http://dvf.ybcxt.top

[R49] awk 带条件
来源：http://njd.mhx1999.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rkk.uphjek.com

[R50] awk 求和
来源：http://wrc.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://ful.9152youxi.cn

[R51] 排序去重取前几
来源：http://lkv.iojbl.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ewj.havefunace.top

[R52] 统计行数
来源：http://sym.yj20258.top

wc -l a.txt
来源：http://amc.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://hlf.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kww.52xcode.cn

[R54] 比较两个文件
来源：http://map.9152youxi.cn

diff a.txt b.txt
来源：http://qlr.bbcook.cn

[R55] 压缩与解压
来源：http://wxa.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wvw.hnxiangtu.top

[R56] 远程拷贝
来源：http://mxu.aibaodan.cn

scp file user@host:/path/
来源：http://xru.jqgfzy.top

[R57] 远程执行命令
来源：http://nzt.wangshuangyany.cn

ssh user@host 'uptime'
来源：http://mcw.ctjpmb.com

[R58] 下载文件
来源：http://hjy.xingfuxueyuan.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jjb.iojbl.cn

[R59] 发 POST JSON
来源：http://evj.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cgc.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://gqz.snrcjt.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jjc.zycfv.cn

[R61] 磁盘占用
来源：http://hzb.tianlin.xyz

df -h;  du -sh *
来源：http://akk.zhoulong.xyz

[R62] 找最占空间的文件
来源：http://ehz.jqgufenzy.top

du -ah . | sort -rh | head -10
来源：http://xor.xingfuxueyuan.xyz

[R63] 内存与进程
来源：http://quc.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://orv.jqgfzy.top

[R64] 结束进程
来源：http://orj.tianlin.xyz

kill -9 $(pgrep -f app.py)
来源：http://arg.sysykeji.top

[R65] 查看端口占用
来源：http://ofa.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pyl.jinqigfzy.top

[R66] 定时任务
来源：http://avj.dianchejie.cn

crontab -e;  crontab -l
来源：http://unq.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://zes.xziqi.cn

openssl rand -hex 16
来源：http://mzz.gaohongyu789.top

[R68] 计算文件校验值
来源：http://efc.xuanzx.com

sha256sum a.txt;  md5sum a.txt
来源：http://fey.yanxiufei.cn

[R69] 生成随机密码
来源：http://qqc.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://tpx.hcnkem.com

[R70] 时间戳与互转
来源：http://ana.aizwys.cn

date +%s;  date -d @1700000000
来源：http://cac.jqgufenzy.top

[R71] 日期格式化
来源：http://rsp.tian-w.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qtb.birdmap.top

[R72] 等待端口就绪
来源：http://hcu.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://uek.yonumen.top

[R73] 分割大日志
来源：http://noi.jlsjyb.cn

split -l 1000 big.log part_
来源：http://pin.xylfe.cn

[R74] 批量重命名
来源：http://dqo.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://njl.xylfe.cn

[R75] 导出环境变量
来源：http://xbd.jinqigfzy.top

export PATH="$HOME/bin:$PATH"
来源：http://bft.sxryk.cn

[R76] 使用临时文件
来源：http://nre.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://seq.yj20258888.top

[R77] 读取用户输入
来源：http://omh.tian-w.cn

read -rp "请输入: " ans
来源：http://hcw.xuanzx.com

[R78] 交互式菜单
来源：http://zrl.dianchejie.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://suz.ydzc1.top

[R79] 解析命令行选项
来源：http://xay.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://myd.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://fjp.xingfuxueyuan.xyz

time ./run.sh
来源：http://lzt.vqdsnc.cn

================================================================================
来源：http://ahy.yueranfly.top

S. C / C++ 专题
来源：http://xuh.xziqi.cn

================================================================================
来源：http://gfj.andypj.xyz

[S01] C：Hello World
来源：http://eax.andypj.xyz

#include <stdio.h>
来源：http://zmw.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://qlg.ivvv.top

[S02] C：变量与格式化输出
来源：http://emv.iojbl.cn

int a = 10; printf("%d\n", a);
来源：http://gjg.shangyingyoupin.top

[S03] C：读入整数
来源：http://tbl.jyoumei.cn

int x; scanf("%d", &x);
来源：http://jdm.fktsv.cn

[S04] C：字符串复制
来源：http://yjf.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://bre.ehwqpu.com

[S05] C：字符串长度
来源：http://iih.zhaomingkeji.xyz

strlen(s)
来源：http://hgg.zhixingplan.top

[S06] C：字符串比较
来源：http://yvp.ybcxt.top

strcmp(a, b) == 0
来源：http://tol.xingfuxueyuan.xyz

[S07] C：数组遍历求和
来源：http://vff.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://opr.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://izl.ybcxt.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jig.52xcode.cn

[S09] C：结构体定义与初始化
来源：http://ego.quarkkingdee.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uyq.xylfe.cn

[S10] C：指针与解引用
来源：http://tli.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://fnt.svipenyu.cn

[S11] C：逐行读文件
来源：http://vub.birdmap.top

FILE *f = fopen("a.txt", "r");
来源：http://bgh.kuanghao11.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://umm.dianchejie.cn

fclose(f);
来源：http://mnv.pengpengdd.cyou

[S12] C：写文件
来源：http://kek.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mbf.zhongyouzk.top

[S13] C：宏定义
来源：http://vfp.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hlp.tianlin.xyz

[S14] C：枚举
来源：http://rdq.vehdjk.com

enum Color { RED, GREEN, BLUE };
来源：http://qjw.yfazqb.com

[S15] C：类型转换
来源：http://czs.feifeiyinyue.top

(double) a / b
来源：http://kzc.yueranfly.top

[S16] C：位操作置位
来源：http://mew.zhijiandao.cn

x |= (1 << 3);
来源：http://dki.guowangkeji.top

[S17] C：安全拼接字符串
来源：http://dkp.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lsy.shangyingyoupin.top

[S18] C：命令行参数
来源：http://pdu.vqdsnc.cn

int main(int argc, char **argv)
来源：http://jku.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://tco.shzxlz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ycf.ydzc1.top

[S20] C：二分查找
来源：http://ryg.yuanzhike.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fle.meibo888.top

[S21] C：字符类别判断
来源：http://lzi.cdnleiting.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hot.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://ifx.guowangkeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://uoa.yongpay.top

[S23] C：随机数
来源：http://ofd.yangfankeji.com

srand(time(NULL));  int r = rand() % 100;
来源：http://uah.fehbvm.com

[S24] C：获取本地时间
来源：http://fyz.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nnf.xylfe.cn

[S25] C：内存拷贝
来源：http://dbn.jyoumei.cn

memcpy(dst, src, n);
来源：http://huv.daxiang520.top

[S26] C：内存清零
来源：http://lso.yanxiufei.cn

memset(a, 0, sizeof a);
来源：http://vik.hfpthk.cn

[S27] C：定义常量
来源：http://kvw.cashguo.top

const double PI = 3.14159;
来源：http://jsf.iojbl.cn

[S28] C：静态变量
来源：http://wqe.yongpay.top

static int counter = 0;
来源：http://csi.ppjwa.cn

[S29] C：变参函数
来源：http://xjx.pycfn.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thj.sxryk.cn

[S30] C：头文件保护
来源：http://kwm.jinqigfzy.top

#ifndef X_H
来源：http://jjb.yfazqb.com

#define X_H
来源：http://sdi.xylfe.cn

#endif
来源：http://gab.zdbjq.cn

[S31] C++：Hello World
来源：http://ecz.cdnleiting.top

#include <iostream>
来源：http://whc.chenjidiqi.icu

int main() { std::cout << "Hello\n"; }
来源：http://iax.zhiwuduotai.top

[S32] C++：字符串
来源：http://iqt.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://wsz.jqgfzy.top

[S33] C++：vector 增删
来源：http://leb.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://une.bjfxy.top

[S34] C++：遍历 vector
来源：http://jkd.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://dnd.yuxming.cn

[S35] C++：map
来源：http://kgc.havefunace.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://auf.jlsjyb.cn

[S36] C++：unordered_map
来源：http://opq.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hxy.yonumen.top

[S37] C++：set
来源：http://mew.bjfxy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vse.xylfe.cn

[S38] C++：排序
来源：http://ypm.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://onb.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://gfj.tian-w.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zmi.cucudq.cn

[S40] C++：查找元素
来源：http://rrw.bjfxy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cte.316326.xyz

[S41] C++：类与构造函数
来源：http://sgr.zdbjq.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fxn.hfpthk.cn

[S42] C++：继承与虚函数
来源：http://wku.andypj.xyz

class B : public Base { public: void f() override {} };
来源：http://ana.xuetiantiany.cn

[S43] C++：智能指针
来源：http://hnp.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://exv.quarkkingdee.top

[S44] C++：引用传参
来源：http://sri.ehwqpu.com

void inc(int &x) { ++x; }
来源：http://bai.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://srr.shangyingyoupin.top

auto add = [](int a, int b) { return a + b; };
来源：http://bkb.jyoumei.cn

[S46] C++：函数模板
来源：http://klk.xuetiantiany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mqm.zhixingplan.top

[S47] C++：结构化绑定遍历
来源：http://trl.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zsy.guowangkeji.top

[S48] C++：逐行读文件
来源：http://njo.jqgfzy.top

std::ifstream in("a.txt");  std::string line;
来源：http://ekk.hnqzz.top

while (std::getline(in, line)) { }
来源：http://qpu.zhaomingkeji.xyz

[S49] C++：写文件
来源：http://qdp.jyoumei.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vcx.meibo888.top

[S50] C++：格式化数字
来源：http://iem.shangyingyoupin.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sup.fehbvm.com

[S51] C++：显式类型转换
来源：http://leu.shuidangran.top

static_cast<double>(a) / b
来源：http://flr.zhiwuduotai.top

[S52] C++：const 与 noexcept
来源：http://dhg.zhoulong.xyz


<!-- 参考信息 -->