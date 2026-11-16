代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ilt.316326.xyz

[Q75] 日期格式化
来源：http://rvl.52xcode.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bip.yj20258.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ufu.ydjk.org.cn

[Q76] 按天统计
来源：http://xyq.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vlx.bjfxy.top

[Q77] 时间加减
来源：http://kqp.vehdjk.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://top.sxryk.cn

[Q78] 当前时间
来源：http://bgr.jinqigufen.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wxz.jqgfzy.top

[Q79] 字符串拼接
来源：http://xzo.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hlr.fengsongda.top

[Q80] 字符串截取
来源：http://upo.yuxming.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jzz.zhijiandao.cn

[Q81] 字符串替换
来源：http://jyr.jinqigufen.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kwq.fehbvm.com

[Q82] 字符长度与字节长度
来源：http://ypx.hammf.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mmf.ydjk.org.cn

[Q83] 大小写转换
来源：http://kow.svipenyu.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://nwj.tianlin.xyz

[Q84] 去除首尾空格
来源：http://fpy.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://ocv.yuanzhike.top

[Q85] 数值取整
来源：http://jey.uphjek.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bjq.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://kjx.ivvv.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ewc.yonumen.top

[Q87] JSON 字段做条件
来源：http://hfm.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://agq.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://hsx.fzhhl.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rlr.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mmk.dashuyun.cn

[Q89] 判断表是否存在
来源：http://coq.shzxlz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fnk.mhx1999.top

[Q90] 生成序号列
来源：http://xun.ywan-chungtsiang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://isr.nanxinkj.top

================================================================================
来源：http://qqp.zhongyouzk.top

R. Bash 专题
来源：http://snz.zhaomingkeji.xyz

================================================================================
来源：http://fdz.sysykeji.top

[R01] shebang 与严格模式
来源：http://zbs.jinqigufen.top

#!/usr/bin/env bash
来源：http://qsl.shzxlz.cn

set -euo pipefail
来源：http://umh.52xcode.cn

[R02] 变量赋值与使用
来源：http://nyu.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://cil.cdnleiting.top

[R03] 只读变量
来源：http://aay.guannengcc.top

readonly PI=3.14
来源：http://pbd.hysaishi.cn

[R04] 位置参数
来源：http://phc.nanxinkj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wjf.bbcook.cn

[R05] 参数默认值
来源：http://art.svipenyu.cn

name="${1:-default}"
来源：http://zoa.cashguo.top

[R06] 判断命令是否存在
来源：http://kub.yueranfly.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://dgu.ppjwa.cn

[R07] if 判断文件
来源：http://crt.haohaochexian.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rmo.jinqigfzy.top

[R08] 数值比较
来源：http://dbf.guannengcc.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zxs.tianlin.xyz

[R09] 字符串比较
来源：http://nhc.aibaodan.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ppw.nanxinkj.top

[R10] 正则匹配
来源：http://jzf.0kj1m.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hbp.fanxiaobao.xyz

[R11] case 多分支
来源：http://uss.shzxlz.cn

case "$1" in
来源：http://anf.zhixingplan.top

start) echo "启动" ;;
来源：http://dam.ehwqpu.com

stop)  echo "停止" ;;
来源：http://vpm.zycfv.cn

*)     echo "未知命令" ;;
来源：http://xhg.ehwqpu.com

esac
来源：http://gpj.cqqwz.cn

[R12] for 遍历文件
来源：http://iqi.bbcook.cn

for f in *.txt; do echo "$f"; done
来源：http://xur.yangfankeji.com

[R13] for 计数循环
来源：http://xqz.pengpengdd.cyou

for i in {1..10}; do echo "$i"; done
来源：http://jen.0kj1m.cn

[R14] C 风格 for
来源：http://oqf.0kj1m.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bsm.zhaomingkeji.xyz

[R15] while 逐行读文件
来源：http://gqj.zycfv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://nnp.jqgufenzy.top

[R16] until 等待条件
来源：http://llm.wangshuangyany.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bpf.aizwys.cn

[R17] 数组定义与取值
来源：http://hwy.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://aql.zhijiandao.cn

[R18] 遍历数组
来源：http://ute.guowangkeji.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ahe.vehdjk.com

[R19] 数组长度
来源：http://agl.yj202588.top

echo "${#arr[@]}"
来源：http://war.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://ezs.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mms.fehbvm.com

[R21] 字符串长度
来源：http://bhq.ybcxt.top

echo "${#s}"
来源：http://wkf.aibaodan.cn

[R22] 截取子串
来源：http://gji.gotoacloud.top

echo "${s:0:5}"
来源：http://lby.ydjk.org.cn

[R23] 字符串替换
来源：http://ixm.shanyushiyangkeji.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zgx.wangdashe.top

[R24] 大小写转换
来源：http://dru.zhiwuduotai.top

echo "${s^^}"; echo "${s,,}"
来源：http://wrf.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://efi.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://hmk.yuxming.cn

[R26] 命令替换
来源：http://xri.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://dnk.birdmap.top

[R27] 算术展开
来源：http://chh.andypj.xyz

echo $((1 + 2 * 3))
来源：http://kjd.pengpengdd.cyou

[R28] 浮点运算
来源：http://rej.ivvv.top

echo "scale=2; 10/3" | bc
来源：http://yui.hnxiangtu.top

[R29] 定义函数
来源：http://xnv.birdmap.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gtx.birdmap.top

[R30] 函数返回状态码
来源：http://mtv.jiagoushi.top

f() { return 0; }; f || echo "失败了"
来源：http://uih.andypj.xyz

[R31] 局部变量
来源：http://rxt.0kj1m.cn

f() { local x=1; echo "$x"; }
来源：http://nis.shanyushiyangkeji.top

[R32] 参数个数校验
来源：http://srn.jqgfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xnk.xinyue.icu

[R33] 捕获错误并提示行号
来源：http://ura.pengpengdd.cyou

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gss.tarul.cn

[R34] 退出时清理
来源：http://eoq.fengsongda.top

trap 'rm -f "$tmp"' EXIT
来源：http://vfv.xylfe.cn

[R35] 后台执行并等待
来源：http://ljo.guannengcc.top

sleep 5 & pid=$!; wait "$pid"
来源：http://pvl.ppjwa.cn

[R36] 并发执行多个任务
来源：http://ykq.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hhh.nanxuanxn.top

[R37] 把输出赋给变量
来源：http://aap.guowangkeji.top

files=$(ls -1)
来源：http://ufs.tarul.cn

[R38] 管道串联
来源：http://xug.sxryk.cn

cat a.txt | grep -i error | wc -l
来源：http://vub.tanke756.top

[R39] 重定向标准输出与错误
来源：http://jzg.yuanzhike.top

cmd > out.log 2>&1
来源：http://zsc.jinghuilouyu.cn

[R40] 追加写日志
来源：http://hck.xinyue.icu

echo "log" >> out.log
来源：http://umb.yangfankeji.com

[R41] 丢弃输出
来源：http://tpe.jqgufenzy.top

cmd >/dev/null 2>&1
来源：http://srr.yueranfly.top

[R42] 输入重定向
来源：http://wlf.0kj1m.cn

wc -l < a.txt
来源：http://jhw.fengsongda.top

[R43] 按名字查找文件
来源：http://fim.nanxuanxn.top

find . -name "*.log" -type f
来源：http://muy.redwolf501.top

[R44] 按修改时间查找
来源：http://bvv.jiagoushi.top

find . -mtime -7 -type f
来源：http://vmh.nwbrower.top

[R45] 批量删除
来源：http://oyz.hongshengwenyu.top

find . -name "*.tmp" -delete
来源：http://jms.zycfv.cn

[R46] 递归替换文件内容
来源：http://cfi.ppjwa.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mdt.zhijiandao.cn

[R47] sed 单行替换
来源：http://hei.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://xga.tianlin.xyz

[R48] awk 取指定列
来源：http://wnz.redwolf501.top

awk '{print $1, $3}' a.txt
来源：http://yni.guowangkeji.top

[R49] awk 带条件
来源：http://toz.epnwcf.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ljr.jlsjyb.cn

[R50] awk 求和
来源：http://fqy.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://nls.vqdsnc.cn

[R51] 排序去重取前几
来源：http://afd.hfpthk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hps.hesvh.cn

[R52] 统计行数
来源：http://aks.zhiwuduotai.top

wc -l a.txt
来源：http://aix.andypj.xyz

[R53] 查看文件头与实时尾
来源：http://brt.nanxuanxn.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vij.mhx1999.top

[R54] 比较两个文件
来源：http://ltl.yanxiufei.cn

diff a.txt b.txt
来源：http://dzx.ydzc1.top

[R55] 压缩与解压
来源：http://lmj.tanke756.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bol.yueranfly.top

[R56] 远程拷贝
来源：http://ufr.andypj.xyz

scp file user@host:/path/
来源：http://pmd.zhijiandao.cn

[R57] 远程执行命令
来源：http://zgl.cheryme.top

ssh user@host 'uptime'
来源：http://vfc.redwolf501.top

[R58] 下载文件
来源：http://aol.chenlongwang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lof.c1oappe.top

[R59] 发 POST JSON
来源：http://lzv.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ufi.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://gng.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gxf.cashguo.top

[R61] 磁盘占用
来源：http://jcz.ybcxt.top

df -h;  du -sh *
来源：http://wms.yangfankeji.com

[R62] 找最占空间的文件
来源：http://elc.xinyue.icu

du -ah . | sort -rh | head -10
来源：http://zlz.zhaomingkeji.xyz

[R63] 内存与进程
来源：http://hvx.ppjwa.cn

free -h;  ps aux | grep nginx
来源：http://kde.hnxiangtu.top

[R64] 结束进程
来源：http://der.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://hrx.haohaochexian.top

[R65] 查看端口占用
来源：http://tpc.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hkd.jqgfzy.top

[R66] 定时任务
来源：http://era.jqgufenzy.top

crontab -e;  crontab -l
来源：http://scc.daxiang520.top

[R67] 生成随机十六进制串
来源：http://tig.yonumen.top

openssl rand -hex 16
来源：http://txr.hesvh.cn

[R68] 计算文件校验值
来源：http://set.cdnleiting.top

sha256sum a.txt;  md5sum a.txt
来源：http://gby.guowangkeji.top

[R69] 生成随机密码
来源：http://klu.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://ylx.aibaodan.cn

[R70] 时间戳与互转
来源：http://qfs.hnqzz.top

date +%s;  date -d @1700000000
来源：http://siw.quarkkingdee.top

[R71] 日期格式化
来源：http://jky.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://voh.tarul.cn

[R72] 等待端口就绪
来源：http://ifh.yj202588.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mxr.sufxvd.cn

[R73] 分割大日志
来源：http://bpk.zhiwuduotai.top

split -l 1000 big.log part_
来源：http://sjp.jqgufenzy.top

[R74] 批量重命名
来源：http://nlx.bjfxy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cnd.cheryme.top

[R75] 导出环境变量
来源：http://knp.xinyue.icu

export PATH="$HOME/bin:$PATH"
来源：http://knt.ctjpmb.com

[R76] 使用临时文件
来源：http://xlf.9152youxi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://btd.yanxiufei.cn

[R77] 读取用户输入
来源：http://lli.c1oappe.top

read -rp "请输入: " ans
来源：http://neg.havefunace.top

[R78] 交互式菜单
来源：http://pca.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qlj.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://cau.mhx1999.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ouo.zhixingplan.top

[R80] 查看脚本执行耗时
来源：http://yhz.pycfn.com

time ./run.sh
来源：http://lqt.iojbl.cn

================================================================================
来源：http://cki.zycfv.cn

S. C / C++ 专题
来源：http://qxi.gotoacloud.top

================================================================================
来源：http://oev.fengsongda.top

[S01] C：Hello World
来源：http://kpw.cucudq.cn

#include <stdio.h>
来源：http://tzf.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uje.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://zaj.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://uph.jinyuanbaomall.cn

[S03] C：读入整数
来源：http://oao.sysykeji.top

int x; scanf("%d", &x);
来源：http://iwf.aizwys.cn

[S04] C：字符串复制
来源：http://hyt.haohaochexian.top

char dst[32]; strcpy(dst, "hi");
来源：http://ikd.pengpengdd.cyou

[S05] C：字符串长度
来源：http://sbp.feifeiyinyue.top

strlen(s)
来源：http://psh.fanxiaobao.xyz

[S06] C：字符串比较
来源：http://qwj.uphjek.com

strcmp(a, b) == 0
来源：http://bkp.hammf.cn

[S07] C：数组遍历求和
来源：http://dpx.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ekj.uphjek.com

[S08] C：动态内存分配与释放
来源：http://afs.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zma.jianghu66.top

[S09] C：结构体定义与初始化
来源：http://hqd.shangyingyoupin.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bht.sweek.top

[S10] C：指针与解引用
来源：http://ttr.fktsv.cn

int *p = &a;  *p = 5;
来源：http://djk.zhaomingkeji.xyz

[S11] C：逐行读文件
来源：http://ybc.zycfv.cn

FILE *f = fopen("a.txt", "r");
来源：http://nqa.aizwys.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nrn.c1oappe.top

fclose(f);
来源：http://cts.yongpay.top

[S12] C：写文件
来源：http://dpd.vehdjk.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rvo.nanxinkj.top

[S13] C：宏定义
来源：http://wak.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dyb.iojbl.cn

[S14] C：枚举
来源：http://agq.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://uyo.zdqjudy.top

[S15] C：类型转换
来源：http://mms.fktsv.cn

(double) a / b
来源：http://rjc.fengsongda.top

[S16] C：位操作置位
来源：http://kkj.daxiang520.top

x |= (1 << 3);
来源：http://iip.jinqigufen.top

[S17] C：安全拼接字符串
来源：http://zwr.hongshengwenyu.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://drk.mhx1999.top

[S18] C：命令行参数
来源：http://qsg.c1oappe.top

int main(int argc, char **argv)
来源：http://evc.tanke756.top

[S19] C：快速排序
来源：http://vpg.nanxinkj.top

qsort(a, n, sizeof(int), cmp);
来源：http://spw.ivvv.top

[S20] C：二分查找
来源：http://oec.yj202588.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vtg.hywenlv.cn

[S21] C：字符类别判断
来源：http://dut.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rvt.yuxming.cn

[S22] C：字符串转数字
来源：http://fwe.sweek.top

atoi("42");  strtod("3.14", NULL);
来源：http://gpx.xuetiantiany.cn

[S23] C：随机数
来源：http://ruw.xuanzx.com

srand(time(NULL));  int r = rand() % 100;
来源：http://yux.meibo888.top

[S24] C：获取本地时间
来源：http://zaz.fehbvm.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pjz.9152youxi.cn

[S25] C：内存拷贝
来源：http://evj.zdbjq.cn

memcpy(dst, src, n);
来源：http://ylj.gogol.net.cn

[S26] C：内存清零
来源：http://buk.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://cqx.ywan-chungtsiang.top

[S27] C：定义常量
来源：http://apj.cashguo.top

const double PI = 3.14159;
来源：http://qvx.guowangkeji.top

[S28] C：静态变量
来源：http://sqf.daxiang520.top

static int counter = 0;
来源：http://lti.yuanzhike.top

[S29] C：变参函数
来源：http://bpd.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ake.sufxvd.cn

[S30] C：头文件保护
来源：http://acl.9152youxi.cn

#ifndef X_H
来源：http://fpa.aibaodan.cn

#define X_H
来源：http://jjr.zhaomingkeji.xyz

#endif
来源：http://vat.wangshuangyany.cn

[S31] C++：Hello World
来源：http://ukm.tarul.cn

#include <iostream>
来源：http://sfe.ywan-chungtsiang.top

int main() { std::cout << "Hello\n"; }
来源：http://sbx.guannengcc.top

[S32] C++：字符串
来源：http://hmr.yonumen.top

std::string s = "hi";  s += "!";
来源：http://ckf.fengsongda.top

[S33] C++：vector 增删
来源：http://uha.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://igo.sufxvd.cn

[S34] C++：遍历 vector
来源：http://qur.gzhubu.top

for (auto &x : v) { std::cout << x; }
来源：http://frd.yonumen.top

[S35] C++：map
来源：http://cfg.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eii.daria6918.cn

[S36] C++：unordered_map
来源：http://lwd.jinghuilouyu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bmo.zdqjudy.top

[S37] C++：set
来源：http://jiu.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lvv.sysykeji.top

[S38] C++：排序
来源：http://gyl.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://xvl.nanxuanxn.top

[S39] C++：自定义比较器排序
来源：http://tei.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://guc.redwolf501.top

[S40] C++：查找元素
来源：http://emt.yangfankeji.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oej.vehdjk.com

[S41] C++：类与构造函数
来源：http://tff.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pya.c1oappe.top

[S42] C++：继承与虚函数
来源：http://eia.bbcook.cn

class B : public Base { public: void f() override {} };
来源：http://ede.iojbl.cn

[S43] C++：智能指针
来源：http://atg.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://bdi.ivvv.top

[S44] C++：引用传参
来源：http://bhp.shanyushiyangkeji.top

void inc(int &x) { ++x; }
来源：http://jyp.jinyuanbaomall.cn


<!-- 参考信息 -->