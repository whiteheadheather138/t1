代发 wailian999

[Q80] 字符串截取
来源：http://bfr.epnwcf.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wuz.ywan-chungtsiang.top

[Q81] 字符串替换
来源：http://wha.gotoacloud.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iea.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://efe.jyoumei.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rfj.shanyushiyangkeji.top

[Q83] 大小写转换
来源：http://tss.feifeiyinyue.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://aic.yueranfly.top

[Q84] 去除首尾空格
来源：http://sfu.zhiwuduotai.top

SELECT TRIM(name) FROM users;
来源：http://bkc.fanxiaobao.xyz

[Q85] 数值取整
来源：http://ylh.jqgfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wgj.gotoacloud.top

[Q86] 读取 JSON 字段
来源：http://dak.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qcj.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://wye.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://eei.ywan-chungtsiang.top

[Q88] 行转列（条件聚合）
来源：http://rss.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ndk.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ewo.andypj.xyz

[Q89] 判断表是否存在
来源：http://edz.quarkkingdee.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://yas.iojbl.cn

[Q90] 生成序号列
来源：http://qxi.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://waz.yvedp.cn

================================================================================
来源：http://hsx.chenlongwang.top

R. Bash 专题
来源：http://ezx.hnxiangtu.top

================================================================================
来源：http://zev.ppjwa.cn

[R01] shebang 与严格模式
来源：http://prc.shzxlz.cn

#!/usr/bin/env bash
来源：http://aha.hcnkem.com

set -euo pipefail
来源：http://wbv.bbcook.cn

[R02] 变量赋值与使用
来源：http://qup.sysykeji.top

name="Tom"; echo "$name"
来源：http://bgp.gogol.net.cn

[R03] 只读变量
来源：http://wbb.jianghu66.top

readonly PI=3.14
来源：http://qjn.zycfv.cn

[R04] 位置参数
来源：http://opi.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://kta.xziqi.cn

[R05] 参数默认值
来源：http://kkv.jianghu66.top

name="${1:-default}"
来源：http://pja.dianchejie.cn

[R06] 判断命令是否存在
来源：http://jty.yvedp.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jdh.nanxuanxn.top

[R07] if 判断文件
来源：http://pwg.zhoulong.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jnr.xziqi.cn

[R08] 数值比较
来源：http://gib.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ilo.hywenlv.cn

[R09] 字符串比较
来源：http://wof.yuxming.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qle.pengpengdd.cyou

[R10] 正则匹配
来源：http://dsq.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://yfc.yongpay.top

[R11] case 多分支
来源：http://skz.ctjpmb.com

case "$1" in
来源：http://pkx.hfpthk.cn

start) echo "启动" ;;
来源：http://xbo.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://aqt.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://dff.c1oappe.top

esac
来源：http://dcg.kuanghao11.cn

[R12] for 遍历文件
来源：http://qun.pycfn.com

for f in *.txt; do echo "$f"; done
来源：http://utd.xylfe.cn

[R13] for 计数循环
来源：http://rdb.fktsv.cn

for i in {1..10}; do echo "$i"; done
来源：http://sqe.smart0.xyz

[R14] C 风格 for
来源：http://qku.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://aee.redwolf501.top

[R15] while 逐行读文件
来源：http://tun.shuidangran.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qkm.jinqigfzy.top

[R16] until 等待条件
来源：http://tcf.cashguo.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fru.jinghuilouyu.cn

[R17] 数组定义与取值
来源：http://cpo.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://sxx.hysaishi.cn

[R18] 遍历数组
来源：http://rsb.birdmap.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gdm.sxryk.cn

[R19] 数组长度
来源：http://ubz.epnwcf.com

echo "${#arr[@]}"
来源：http://nqd.daria6918.cn

[R20] 关联数组（字典）
来源：http://hsv.fzhhl.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kxi.52xcode.cn

[R21] 字符串长度
来源：http://bor.cucudq.cn

echo "${#s}"
来源：http://zjc.ybcxt.top

[R22] 截取子串
来源：http://qpq.sweek.top

echo "${s:0:5}"
来源：http://tzj.cqqwz.cn

[R23] 字符串替换
来源：http://lcv.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://frd.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://wid.jqgfzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://quc.vehdjk.com

[R25] 去后缀 / 去前缀
来源：http://xoy.hnqzz.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lqv.shanyushiyangkeji.top

[R26] 命令替换
来源：http://dxq.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://euo.yonumen.top

[R27] 算术展开
来源：http://ncr.tarul.cn

echo $((1 + 2 * 3))
来源：http://dhf.zhiwuduotai.top

[R28] 浮点运算
来源：http://fhs.hongshengwenyu.top

echo "scale=2; 10/3" | bc
来源：http://tgn.vqdsnc.cn

[R29] 定义函数
来源：http://qen.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dpz.bbcook.cn

[R30] 函数返回状态码
来源：http://mmc.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://tqe.daria6918.cn

[R31] 局部变量
来源：http://ati.sysykeji.top

f() { local x=1; echo "$x"; }
来源：http://sbv.ivvv.top

[R32] 参数个数校验
来源：http://lyy.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ggo.cashguo.top

[R33] 捕获错误并提示行号
来源：http://lir.dianchejie.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nfc.daria6918.cn

[R34] 退出时清理
来源：http://ksm.vehdjk.com

trap 'rm -f "$tmp"' EXIT
来源：http://qzs.yj20258888.top

[R35] 后台执行并等待
来源：http://hgb.tian-w.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://usl.tian-w.cn

[R36] 并发执行多个任务
来源：http://uhq.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://khp.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://mes.redwolf501.top

files=$(ls -1)
来源：http://vsy.sufxvd.cn

[R38] 管道串联
来源：http://fpw.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://phm.hywenlv.cn

[R39] 重定向标准输出与错误
来源：http://zuw.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://hrj.xziqi.cn

[R40] 追加写日志
来源：http://bbc.kuanghao11.cn

echo "log" >> out.log
来源：http://wnx.pengpengdd.cyou

[R41] 丢弃输出
来源：http://ybh.fengsongda.top

cmd >/dev/null 2>&1
来源：http://axr.jinqigfzy.top

[R42] 输入重定向
来源：http://isj.ydzc1.top

wc -l < a.txt
来源：http://upv.iojbl.cn

[R43] 按名字查找文件
来源：http://nfy.sufxvd.cn

find . -name "*.log" -type f
来源：http://fgh.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://cfr.zdbjq.cn

find . -mtime -7 -type f
来源：http://kfu.ctjpmb.com

[R45] 批量删除
来源：http://rqh.shuidangran.top

find . -name "*.tmp" -delete
来源：http://sms.cucudq.cn

[R46] 递归替换文件内容
来源：http://tzh.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tii.hywenlv.cn

[R47] sed 单行替换
来源：http://zib.fzhhl.top

sed -i 's/foo/bar/g' a.txt
来源：http://rzw.zhijiandao.cn

[R48] awk 取指定列
来源：http://jyr.cdnleiting.top

awk '{print $1, $3}' a.txt
来源：http://asv.gotoacloud.top

[R49] awk 带条件
来源：http://ppe.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xzs.fehbvm.com

[R50] awk 求和
来源：http://twr.xuanzx.com

awk '{s += $2} END {print s}' a.txt
来源：http://fxw.dashuyun.cn

[R51] 排序去重取前几
来源：http://gug.xinyue.icu

sort a.txt | uniq -c | sort -rn | head
来源：http://bzk.sjlbkw.cn

[R52] 统计行数
来源：http://raf.sjlbkw.cn

wc -l a.txt
来源：http://ifx.hcnkem.com

[R53] 查看文件头与实时尾
来源：http://iwy.zhongyouzk.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mny.hesvh.cn

[R54] 比较两个文件
来源：http://ibb.zdbjq.cn

diff a.txt b.txt
来源：http://pqr.aizwys.cn

[R55] 压缩与解压
来源：http://ejf.aizwys.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kqi.haohaochexian.top

[R56] 远程拷贝
来源：http://fpi.iojbl.cn

scp file user@host:/path/
来源：http://all.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://dbd.xuetiantiany.cn

ssh user@host 'uptime'
来源：http://lim.52xcode.cn

[R58] 下载文件
来源：http://znp.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://liq.ydzc1.top

[R59] 发 POST JSON
来源：http://tyx.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xrj.hcnkem.com

[R60] 只看 HTTP 状态码
来源：http://kwj.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oep.hysaishi.cn

[R61] 磁盘占用
来源：http://oes.daria6918.cn

df -h;  du -sh *
来源：http://crq.shanyushiyangtech.top

[R62] 找最占空间的文件
来源：http://blo.uphjek.com

du -ah . | sort -rh | head -10
来源：http://vfk.jqgfzy.top

[R63] 内存与进程
来源：http://rfv.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://znf.cqqwz.cn

[R64] 结束进程
来源：http://eov.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://ukn.wangshuangyany.cn

[R65] 查看端口占用
来源：http://oka.uphjek.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ums.jqgfzy.top

[R66] 定时任务
来源：http://jpr.sjlbkw.cn

crontab -e;  crontab -l
来源：http://yri.andypj.xyz

[R67] 生成随机十六进制串
来源：http://klk.xuanzx.com

openssl rand -hex 16
来源：http://cgm.ivvv.top

[R68] 计算文件校验值
来源：http://vkg.bjfxy.top

sha256sum a.txt;  md5sum a.txt
来源：http://vwd.zhengqikj.top

[R69] 生成随机密码
来源：http://php.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://hng.nwbrower.top

[R70] 时间戳与互转
来源：http://oig.zdbjq.cn

date +%s;  date -d @1700000000
来源：http://lzf.quarkkingdee.top

[R71] 日期格式化
来源：http://alu.ppjwa.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://goh.hfpthk.cn

[R72] 等待端口就绪
来源：http://msk.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ewd.jinyuanbaomall.cn

[R73] 分割大日志
来源：http://nze.cucudq.cn

split -l 1000 big.log part_
来源：http://ndz.yongpay.top

[R74] 批量重命名
来源：http://iwh.jqgfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vth.sweek.top

[R75] 导出环境变量
来源：http://ict.ydzc1.top

export PATH="$HOME/bin:$PATH"
来源：http://trg.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://wwa.52xcode.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hoe.yangfankeji.com

[R77] 读取用户输入
来源：http://smt.zhixingplan.top

read -rp "请输入: " ans
来源：http://zpc.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://rlt.gzhubu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vqx.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://any.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kwa.jinqigfzy.top

[R80] 查看脚本执行耗时
来源：http://ngb.zycfv.cn

time ./run.sh
来源：http://ijd.0kj1m.cn

================================================================================
来源：http://tnf.aizwys.cn

S. C / C++ 专题
来源：http://dcp.zdqjudy.top

================================================================================
来源：http://tnb.sweek.top

[S01] C：Hello World
来源：http://tjl.shangyingyoupin.top

#include <stdio.h>
来源：http://hpn.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mhj.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://owe.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://pdk.gotoacloud.top

[S03] C：读入整数
来源：http://fcw.guannengcc.top

int x; scanf("%d", &x);
来源：http://hmw.cqqwz.cn

[S04] C：字符串复制
来源：http://lav.jqgfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://yma.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://zux.cheryme.top

strlen(s)
来源：http://xuj.jyoumei.cn

[S06] C：字符串比较
来源：http://xxi.snrcjt.cn

strcmp(a, b) == 0
来源：http://skv.shanyushiyangtech.top

[S07] C：数组遍历求和
来源：http://zxs.wangshuangyany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jst.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://kst.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dxw.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://yno.jyoumei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rex.yanxiufei.cn

[S10] C：指针与解引用
来源：http://xfi.hammf.cn

int *p = &a;  *p = 5;
来源：http://rhv.jqgufenzy.top

[S11] C：逐行读文件
来源：http://xjk.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://prr.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://syu.yonumen.top

fclose(f);
来源：http://dxn.smart0.xyz

[S12] C：写文件
来源：http://bkd.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hez.sysykeji.top

[S13] C：宏定义
来源：http://ofu.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mwc.zhoulong.xyz

[S14] C：枚举
来源：http://key.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://yfj.sufxvd.cn

[S15] C：类型转换
来源：http://ipd.cucudq.cn

(double) a / b
来源：http://hgv.yueranfly.top

[S16] C：位操作置位
来源：http://zxw.pengpengdd.cyou

x |= (1 << 3);
来源：http://rod.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://zdk.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vca.xziqi.cn

[S18] C：命令行参数
来源：http://rma.gotoacloud.top

int main(int argc, char **argv)
来源：http://vdv.ydjk.org.cn

[S19] C：快速排序
来源：http://zvr.hnxiangtu.top

qsort(a, n, sizeof(int), cmp);
来源：http://aio.tianlin.xyz

[S20] C：二分查找
来源：http://dqq.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://unt.nanxuanxn.top

[S21] C：字符类别判断
来源：http://lgw.svipenyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://idw.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://qpj.zdbjq.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ext.chenzaomai.com

[S23] C：随机数
来源：http://hjf.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://skz.hcnkem.com

[S24] C：获取本地时间
来源：http://vvw.bbcook.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uge.yj20258.top

[S25] C：内存拷贝
来源：http://tnz.daria6918.cn

memcpy(dst, src, n);
来源：http://vtz.gotoacloud.top

[S26] C：内存清零
来源：http://lis.wangshuangyany.cn

memset(a, 0, sizeof a);
来源：http://bbu.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://dre.nanxuanxn.top

const double PI = 3.14159;
来源：http://muq.sufxvd.cn

[S28] C：静态变量
来源：http://zok.aizwys.cn

static int counter = 0;
来源：http://pka.haohaochexian.top

[S29] C：变参函数
来源：http://kkg.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gpu.birdmap.top

[S30] C：头文件保护
来源：http://qjq.yongpay.top

#ifndef X_H
来源：http://ncb.hcnkem.com

#define X_H
来源：http://vzj.c1oappe.top

#endif
来源：http://sdx.chenlongwang.top

[S31] C++：Hello World
来源：http://pfs.zhengqikj.top

#include <iostream>
来源：http://ajg.jinyuanbaomall.cn

int main() { std::cout << "Hello\n"; }
来源：http://yrd.epnwcf.com

[S32] C++：字符串
来源：http://fgj.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://swn.yj20258.top

[S33] C++：vector 增删
来源：http://sfh.ywan-chungtsiang.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kqw.52xcode.cn

[S34] C++：遍历 vector
来源：http://ibq.gotoacloud.top

for (auto &x : v) { std::cout << x; }
来源：http://hsn.hesvh.cn

[S35] C++：map
来源：http://hgy.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ylh.jinqigfzy.top

[S36] C++：unordered_map
来源：http://cfa.feifeiyinyue.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cic.jinghuilouyu.cn

[S37] C++：set
来源：http://bdw.hcnkem.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mwg.gotoacloud.top

[S38] C++：排序
来源：http://txn.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://cyx.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://xkd.vehdjk.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zkr.shanyushiyangkeji.top

[S40] C++：查找元素
来源：http://tdj.guannengcc.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jzp.ydjk.org.cn

[S41] C++：类与构造函数
来源：http://pas.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rzt.zhijiandao.cn

[S42] C++：继承与虚函数
来源：http://ioy.cqqwz.cn

class B : public Base { public: void f() override {} };
来源：http://dpy.fzhhl.top

[S43] C++：智能指针
来源：http://ptd.jlsjyb.cn

auto p = std::make_unique<int>(5);
来源：http://qfb.jqgufenzy.top

[S44] C++：引用传参
来源：http://iab.xinyue.icu

void inc(int &x) { ++x; }
来源：http://rbf.tian-w.cn

[S45] C++：lambda
来源：http://gvg.yonumen.top

auto add = [](int a, int b) { return a + b; };
来源：http://uuc.gogol.net.cn

[S46] C++：函数模板
来源：http://xoz.uphjek.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://imu.gzhubu.top

[S47] C++：结构化绑定遍历
来源：http://icp.sjlbkw.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ara.redwolf501.top

[S48] C++：逐行读文件
来源：http://vze.yj20258888.top

std::ifstream in("a.txt");  std::string line;
来源：http://gek.fehbvm.com

while (std::getline(in, line)) { }
来源：http://rsv.iojbl.cn

[S49] C++：写文件
来源：http://ysq.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://oeg.yj20258888.top

[S50] C++：格式化数字
来源：http://rju.uphjek.com


<!-- 参考信息 -->