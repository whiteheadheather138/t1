代发 wailian999

[Q78] 当前时间
来源：http://okd.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gqb.hongshengwenyu.top

[Q79] 字符串拼接
来源：http://hnd.andypj.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gtx.316326.xyz

[Q80] 字符串截取
来源：http://qge.jinqigufen.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pmz.ydjk.org.cn

[Q81] 字符串替换
来源：http://fbe.yj20258888.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nxb.yuxming.cn

[Q82] 字符长度与字节长度
来源：http://ski.hcnkem.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bqx.9152youxi.cn

[Q83] 大小写转换
来源：http://tcs.zhaomingkeji.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://arl.sufxvd.cn

[Q84] 去除首尾空格
来源：http://znm.pycfn.com

SELECT TRIM(name) FROM users;
来源：http://klg.ybcxt.top

[Q85] 数值取整
来源：http://sbu.dashuyun.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bqt.zdqjudy.top

[Q86] 读取 JSON 字段
来源：http://hly.jinghuilouyu.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gfc.sysykeji.top

[Q87] JSON 字段做条件
来源：http://ili.quarkkingdee.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ybi.ydzc1.top

[Q88] 行转列（条件聚合）
来源：http://bva.vehdjk.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bhs.hcnkem.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xuy.zhaomingkeji.xyz

[Q89] 判断表是否存在
来源：http://zjb.hysaishi.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://bji.gaohongyu789.top

[Q90] 生成序号列
来源：http://mnw.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://cup.fengsongda.top

================================================================================
来源：http://zdv.hywenlv.cn

R. Bash 专题
来源：http://cur.xingfuxueyuan.xyz

================================================================================
来源：http://vtz.yfazqb.com

[R01] shebang 与严格模式
来源：http://nfq.hywenlv.cn

#!/usr/bin/env bash
来源：http://yia.haohaochexian.top

set -euo pipefail
来源：http://vaq.zhijiandao.cn

[R02] 变量赋值与使用
来源：http://wuv.fzhhl.top

name="Tom"; echo "$name"
来源：http://cdt.yj20258.top

[R03] 只读变量
来源：http://sno.sxryk.cn

readonly PI=3.14
来源：http://bqz.redwolf501.top

[R04] 位置参数
来源：http://gsb.dianchejie.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fxt.cashguo.top

[R05] 参数默认值
来源：http://igz.pycfn.com

name="${1:-default}"
来源：http://aro.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://kmq.guowangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kqe.fanxiaobao.xyz

[R07] if 判断文件
来源：http://rja.sjlbkw.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hzz.daxiang520.top

[R08] 数值比较
来源：http://oct.hysaishi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lhg.yonumen.top

[R09] 字符串比较
来源：http://uho.zhongyouzk.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sth.xylfe.cn

[R10] 正则匹配
来源：http://xcl.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hom.hesvh.cn

[R11] case 多分支
来源：http://qiw.yj20258888.top

case "$1" in
来源：http://fej.tanke756.top

start) echo "启动" ;;
来源：http://hmr.cashguo.top

stop)  echo "停止" ;;
来源：http://sbh.zhoulong.xyz

*)     echo "未知命令" ;;
来源：http://swp.zdbjq.cn

esac
来源：http://axu.fengsongda.top

[R12] for 遍历文件
来源：http://ehe.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://gkc.zhijiandao.cn

[R13] for 计数循环
来源：http://etk.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://uzp.9152youxi.cn

[R14] C 风格 for
来源：http://zzx.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qqy.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://pfr.cqqwz.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jpz.shanyushiyangtech.top

[R16] until 等待条件
来源：http://pie.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ynd.pengpengdd.cyou

[R17] 数组定义与取值
来源：http://gmz.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://pkm.ivvv.top

[R18] 遍历数组
来源：http://dyp.ctjpmb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rcm.tarul.cn

[R19] 数组长度
来源：http://hwh.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://vxo.jinyuanbaomall.cn

[R20] 关联数组（字典）
来源：http://uhz.jinqigufen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ktx.fehbvm.com

[R21] 字符串长度
来源：http://mdz.fzhhl.top

echo "${#s}"
来源：http://hyw.tanke756.top

[R22] 截取子串
来源：http://yaq.zhengqikj.top

echo "${s:0:5}"
来源：http://xpa.feifeiyinyue.top

[R23] 字符串替换
来源：http://dby.zhaomingkeji.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rcm.chenlongwang.top

[R24] 大小写转换
来源：http://zhc.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://oop.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://goa.9152youxi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://llz.jinqigufen.top

[R26] 命令替换
来源：http://fio.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://omr.tanke756.top

[R27] 算术展开
来源：http://fox.pengpengdd.cyou

echo $((1 + 2 * 3))
来源：http://gaw.ppjwa.cn

[R28] 浮点运算
来源：http://fde.316326.xyz

echo "scale=2; 10/3" | bc
来源：http://tme.ywan-chungtsiang.top

[R29] 定义函数
来源：http://wff.yvedp.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kzu.hywenlv.cn

[R30] 函数返回状态码
来源：http://pxr.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://nyk.hysaishi.cn

[R31] 局部变量
来源：http://rfb.yueranfly.top

f() { local x=1; echo "$x"; }
来源：http://ceg.52xcode.cn

[R32] 参数个数校验
来源：http://dop.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oma.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://suf.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mvy.jyoumei.cn

[R34] 退出时清理
来源：http://qkg.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xzf.nanxuanxn.top

[R35] 后台执行并等待
来源：http://ugf.zhixingplan.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vhi.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://uuv.xinyue.icu

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xmo.9152youxi.cn

[R37] 把输出赋给变量
来源：http://nwp.andypj.xyz

files=$(ls -1)
来源：http://ipo.hywenlv.cn

[R38] 管道串联
来源：http://crl.zycfv.cn

cat a.txt | grep -i error | wc -l
来源：http://yeb.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://enr.ivvv.top

cmd > out.log 2>&1
来源：http://xdq.nwbrower.top

[R40] 追加写日志
来源：http://jyn.redwolf501.top

echo "log" >> out.log
来源：http://ajn.zhongyouzk.top

[R41] 丢弃输出
来源：http://ugf.andypj.xyz

cmd >/dev/null 2>&1
来源：http://enx.fktsv.cn

[R42] 输入重定向
来源：http://bey.guowangkeji.top

wc -l < a.txt
来源：http://tov.fehbvm.com

[R43] 按名字查找文件
来源：http://cwf.ydzc1.top

find . -name "*.log" -type f
来源：http://gdr.hcnkem.com

[R44] 按修改时间查找
来源：http://dpo.yfazqb.com

find . -mtime -7 -type f
来源：http://zcq.meibo888.top

[R45] 批量删除
来源：http://cfh.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://sux.redwolf501.top

[R46] 递归替换文件内容
来源：http://csj.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iqg.xylfe.cn

[R47] sed 单行替换
来源：http://khy.cdnleiting.top

sed -i 's/foo/bar/g' a.txt
来源：http://rxb.yj202588.top

[R48] awk 取指定列
来源：http://tef.meibo888.top

awk '{print $1, $3}' a.txt
来源：http://dez.tianlin.xyz

[R49] awk 带条件
来源：http://yec.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vtt.yj20258888.top

[R50] awk 求和
来源：http://cjh.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://dkk.gogol.net.cn

[R51] 排序去重取前几
来源：http://bcr.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fao.meibo888.top

[R52] 统计行数
来源：http://ivx.ydzc1.top

wc -l a.txt
来源：http://fiz.yuanzhike.top

[R53] 查看文件头与实时尾
来源：http://lep.jqgfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pim.ehwqpu.com

[R54] 比较两个文件
来源：http://rvh.tian-w.cn

diff a.txt b.txt
来源：http://jho.hongshengwenyu.top

[R55] 压缩与解压
来源：http://alm.guowangkeji.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://crj.hysaishi.cn

[R56] 远程拷贝
来源：http://lwp.sxryk.cn

scp file user@host:/path/
来源：http://smc.cqqwz.cn

[R57] 远程执行命令
来源：http://sgd.zhengqikj.top

ssh user@host 'uptime'
来源：http://laz.chenjidiqi.icu

[R58] 下载文件
来源：http://hdu.andypj.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gux.ivvv.top

[R59] 发 POST JSON
来源：http://qgt.dashuyun.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cyp.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://cnf.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bkt.zdbjq.cn

[R61] 磁盘占用
来源：http://nrx.cdnleiting.top

df -h;  du -sh *
来源：http://pxx.ctjpmb.com

[R62] 找最占空间的文件
来源：http://oqh.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://rny.jinyuanbaomall.cn

[R63] 内存与进程
来源：http://jye.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://axc.jinqigfzy.top

[R64] 结束进程
来源：http://exo.cdnleiting.top

kill -9 $(pgrep -f app.py)
来源：http://lvn.cqqwz.cn

[R65] 查看端口占用
来源：http://yce.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gsw.wangdashe.top

[R66] 定时任务
来源：http://ogj.vehdjk.com

crontab -e;  crontab -l
来源：http://thm.daxiang520.top

[R67] 生成随机十六进制串
来源：http://erh.zhoulong.xyz

openssl rand -hex 16
来源：http://guo.jyoumei.cn

[R68] 计算文件校验值
来源：http://xxm.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jgi.mhx1999.top

[R69] 生成随机密码
来源：http://xqc.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://rif.yangfankeji.com

[R70] 时间戳与互转
来源：http://prp.ybcxt.top

date +%s;  date -d @1700000000
来源：http://fmc.tanke756.top

[R71] 日期格式化
来源：http://qpw.jianghu66.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ujf.snrcjt.cn

[R72] 等待端口就绪
来源：http://axj.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yxx.zhixingplan.top

[R73] 分割大日志
来源：http://nuo.xinyue.icu

split -l 1000 big.log part_
来源：http://iji.zdbjq.cn

[R74] 批量重命名
来源：http://xuf.redwolf501.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bkf.52xcode.cn

[R75] 导出环境变量
来源：http://ani.fanxiaobao.xyz

export PATH="$HOME/bin:$PATH"
来源：http://hyp.fengsongda.top

[R76] 使用临时文件
来源：http://fiu.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ais.daria6918.cn

[R77] 读取用户输入
来源：http://bnz.yonumen.top

read -rp "请输入: " ans
来源：http://iar.vehdjk.com

[R78] 交互式菜单
来源：http://ril.zhixingplan.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rql.zhongyouzk.top

[R79] 解析命令行选项
来源：http://sth.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ujl.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://klj.dianchejie.cn

time ./run.sh
来源：http://xby.zhaomingkeji.xyz

================================================================================
来源：http://lpt.jiagoushi.top

S. C / C++ 专题
来源：http://bjk.fehbvm.com

================================================================================
来源：http://eoa.dashuyun.cn

[S01] C：Hello World
来源：http://axj.jianghu66.top

#include <stdio.h>
来源：http://slt.hywenlv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ztn.snrcjt.cn

[S02] C：变量与格式化输出
来源：http://fzs.zhixingplan.top

int a = 10; printf("%d\n", a);
来源：http://oaz.yvedp.cn

[S03] C：读入整数
来源：http://wkm.yangfankeji.com

int x; scanf("%d", &x);
来源：http://eag.xinyue.icu

[S04] C：字符串复制
来源：http://buf.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://agk.ehwqpu.com

[S05] C：字符串长度
来源：http://ema.kuanghao11.cn

strlen(s)
来源：http://xjt.yueranfly.top

[S06] C：字符串比较
来源：http://liq.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://gdq.hesvh.cn

[S07] C：数组遍历求和
来源：http://tme.andypj.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wav.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://neb.zhaomingkeji.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ums.pycfn.com

[S09] C：结构体定义与初始化
来源：http://kfi.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xdm.zycfv.cn

[S10] C：指针与解引用
来源：http://gjk.yfazqb.com

int *p = &a;  *p = 5;
来源：http://ngh.hesvh.cn

[S11] C：逐行读文件
来源：http://epk.hnxiangtu.top

FILE *f = fopen("a.txt", "r");
来源：http://iww.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://zcm.chenzaomai.com

fclose(f);
来源：http://hma.birdmap.top

[S12] C：写文件
来源：http://zta.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wvj.yuxming.cn

[S13] C：宏定义
来源：http://aui.cqqwz.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://szi.guowangkeji.top

[S14] C：枚举
来源：http://vgo.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://ysq.shuidangran.top

[S15] C：类型转换
来源：http://rez.shanyushiyangtech.top

(double) a / b
来源：http://bep.zhengqikj.top

[S16] C：位操作置位
来源：http://fej.ivvv.top

x |= (1 << 3);
来源：http://dhk.fengsongda.top

[S17] C：安全拼接字符串
来源：http://foi.yongpay.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://elz.tanke756.top

[S18] C：命令行参数
来源：http://ruv.sxryk.cn

int main(int argc, char **argv)
来源：http://nuj.birdmap.top

[S19] C：快速排序
来源：http://dmw.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://nzs.yueranfly.top

[S20] C：二分查找
来源：http://nzw.yuxming.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cfi.cheryme.top

[S21] C：字符类别判断
来源：http://ktj.nanxinkj.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hut.jianghu66.top

[S22] C：字符串转数字
来源：http://dvx.epnwcf.com

atoi("42");  strtod("3.14", NULL);
来源：http://pna.dashuyun.cn

[S23] C：随机数
来源：http://kyv.vehdjk.com

srand(time(NULL));  int r = rand() % 100;
来源：http://jfj.fktsv.cn

[S24] C：获取本地时间
来源：http://ljo.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uyq.yj20258888.top

[S25] C：内存拷贝
来源：http://gtu.zhengqikj.top

memcpy(dst, src, n);
来源：http://zdq.hongshengwenyu.top

[S26] C：内存清零
来源：http://cpo.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://fkg.cashguo.top

[S27] C：定义常量
来源：http://ten.nanxuanxn.top

const double PI = 3.14159;
来源：http://qpw.zhengqikj.top

[S28] C：静态变量
来源：http://cxj.yuanzhike.top

static int counter = 0;
来源：http://yri.shanyushiyangtech.top

[S29] C：变参函数
来源：http://tru.shanyushiyangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jyh.uphjek.com

[S30] C：头文件保护
来源：http://qyu.guannengcc.top

#ifndef X_H
来源：http://nmd.jinqigufen.top

#define X_H
来源：http://fqo.fzhhl.top

#endif
来源：http://wzq.haohaochexian.top

[S31] C++：Hello World
来源：http://noz.jinqigfzy.top

#include <iostream>
来源：http://msq.yanxiufei.cn

int main() { std::cout << "Hello\n"; }
来源：http://sup.xingfuxueyuan.xyz

[S32] C++：字符串
来源：http://kbt.havefunace.top

std::string s = "hi";  s += "!";
来源：http://jyw.yfazqb.com

[S33] C++：vector 增删
来源：http://kqw.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bol.smart0.xyz

[S34] C++：遍历 vector
来源：http://wrj.fanxiaobao.xyz

for (auto &x : v) { std::cout << x; }
来源：http://mpb.cheryme.top

[S35] C++：map
来源：http://ogu.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dxy.chenzaomai.com

[S36] C++：unordered_map
来源：http://vcj.sysykeji.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://voz.gzhubu.top

[S37] C++：set
来源：http://paa.tarul.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://kap.hnqzz.top

[S38] C++：排序
来源：http://plu.jqgfzy.top

std::sort(v.begin(), v.end());
来源：http://ggs.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://tmz.kuanghao11.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qis.shzxlz.cn

[S40] C++：查找元素
来源：http://mlx.hnxiangtu.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hqd.fengsongda.top

[S41] C++：类与构造函数
来源：http://mac.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sfc.andypj.xyz

[S42] C++：继承与虚函数
来源：http://azw.hnxiangtu.top

class B : public Base { public: void f() override {} };
来源：http://dtp.yvedp.cn

[S43] C++：智能指针
来源：http://yqv.hfpthk.cn

auto p = std::make_unique<int>(5);
来源：http://hno.iojbl.cn

[S44] C++：引用传参
来源：http://eym.vehdjk.com

void inc(int &x) { ++x; }
来源：http://kva.zhixingplan.top

[S45] C++：lambda
来源：http://zgj.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://rtw.hywenlv.cn

[S46] C++：函数模板
来源：http://cxn.yongpay.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tzw.feifeiyinyue.top

[S47] C++：结构化绑定遍历
来源：http://pcz.ydzc1.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://voi.nwbrower.top

[S48] C++：逐行读文件
来源：http://mhw.0kj1m.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wwi.pengpengdd.cyou


<!-- 参考信息 -->