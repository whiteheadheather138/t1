代发 wailian999

SHOW INDEX FROM users;
来源：http://xav.hnxiangtu.top

[Q73] 查看表状态
来源：http://hsw.hammf.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mkb.sysykeji.top

[Q74] 强制使用索引
来源：http://vrt.shuidangran.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hjo.daria6918.cn

[Q75] 日期格式化
来源：http://fkc.yueranfly.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kdy.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cot.sysykeji.top

[Q76] 按天统计
来源：http://iev.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://bog.zhijiandao.cn

[Q77] 时间加减
来源：http://bhx.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hdk.bbcook.cn

[Q78] 当前时间
来源：http://xip.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qvn.gotoacloud.top

[Q79] 字符串拼接
来源：http://mbq.ivvv.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hag.zhaomingkeji.xyz

[Q80] 字符串截取
来源：http://xvv.fengsongda.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://toj.cdnleiting.top

[Q81] 字符串替换
来源：http://ymw.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rnk.pengpengdd.cyou

[Q82] 字符长度与字节长度
来源：http://evp.yvedp.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hyo.hnqzz.top

[Q83] 大小写转换
来源：http://lol.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rwv.0kj1m.cn

[Q84] 去除首尾空格
来源：http://jkg.hesvh.cn

SELECT TRIM(name) FROM users;
来源：http://wik.zhoulong.xyz

[Q85] 数值取整
来源：http://rjf.pengpengdd.cyou

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zwf.hnxiangtu.top

[Q86] 读取 JSON 字段
来源：http://viy.jqgfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gci.yangfankeji.com

[Q87] JSON 字段做条件
来源：http://ixs.xuetiantiany.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://myc.cqqwz.cn

[Q88] 行转列（条件聚合）
来源：http://jgo.kuanghao11.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xrx.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hcz.ydjk.org.cn

[Q89] 判断表是否存在
来源：http://wjj.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hiw.jqgfzy.top

[Q90] 生成序号列
来源：http://oul.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jne.daria6918.cn

================================================================================
来源：http://ddy.cashguo.top

R. Bash 专题
来源：http://jdl.redwolf501.top

================================================================================
来源：http://uoq.dashuyun.cn

[R01] shebang 与严格模式
来源：http://czq.316326.xyz

#!/usr/bin/env bash
来源：http://jfj.xingfuxueyuan.xyz

set -euo pipefail
来源：http://fkp.fengsongda.top

[R02] 变量赋值与使用
来源：http://vqc.smart0.xyz

name="Tom"; echo "$name"
来源：http://huv.quarkkingdee.top

[R03] 只读变量
来源：http://vdw.sufxvd.cn

readonly PI=3.14
来源：http://peh.yonumen.top

[R04] 位置参数
来源：http://ymc.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cgd.chenlongwang.top

[R05] 参数默认值
来源：http://jns.guowangkeji.top

name="${1:-default}"
来源：http://yoh.hnqzz.top

[R06] 判断命令是否存在
来源：http://pgq.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mle.yangfankeji.com

[R07] if 判断文件
来源：http://lut.mhx1999.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ina.pycfn.com

[R08] 数值比较
来源：http://ywx.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uab.xuetiantiany.cn

[R09] 字符串比较
来源：http://nww.ivvv.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bhe.hongshengwenyu.top

[R10] 正则匹配
来源：http://yqz.ivvv.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xxp.zhaomingkeji.xyz

[R11] case 多分支
来源：http://iwt.hongshengwenyu.top

case "$1" in
来源：http://qzb.wangdashe.top

start) echo "启动" ;;
来源：http://kyc.zdqjudy.top

stop)  echo "停止" ;;
来源：http://oxz.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://nff.xziqi.cn

esac
来源：http://kch.iojbl.cn

[R12] for 遍历文件
来源：http://kcu.9152youxi.cn

for f in *.txt; do echo "$f"; done
来源：http://qzc.chenzaomai.com

[R13] for 计数循环
来源：http://inf.ywan-chungtsiang.top

for i in {1..10}; do echo "$i"; done
来源：http://cxz.vqdsnc.cn

[R14] C 风格 for
来源：http://cmk.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jkb.dianchejie.cn

[R15] while 逐行读文件
来源：http://qka.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hqq.fktsv.cn

[R16] until 等待条件
来源：http://esp.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://oci.zycfv.cn

[R17] 数组定义与取值
来源：http://lid.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mfj.kuanghao11.cn

[R18] 遍历数组
来源：http://jgm.hysaishi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tta.c1oappe.top

[R19] 数组长度
来源：http://qrf.shangyingyoupin.top

echo "${#arr[@]}"
来源：http://gag.bbcook.cn

[R20] 关联数组（字典）
来源：http://dde.feifeiyinyue.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xdc.fzhhl.top

[R21] 字符串长度
来源：http://udu.hysaishi.cn

echo "${#s}"
来源：http://qzt.cashguo.top

[R22] 截取子串
来源：http://nwu.xuetiantiany.cn

echo "${s:0:5}"
来源：http://fak.cdnleiting.top

[R23] 字符串替换
来源：http://rwk.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ako.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://wtv.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://htu.tianlin.xyz

[R25] 去后缀 / 去前缀
来源：http://ysm.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://pqd.jiagoushi.top

[R26] 命令替换
来源：http://zcs.hysaishi.cn

now=$(date +%F); echo "$now"
来源：http://hnn.xuetiantiany.cn

[R27] 算术展开
来源：http://jtl.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://bxu.fengsongda.top

[R28] 浮点运算
来源：http://oyh.jqgfzy.top

echo "scale=2; 10/3" | bc
来源：http://qts.tian-w.cn

[R29] 定义函数
来源：http://wfb.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fft.hywenlv.cn

[R30] 函数返回状态码
来源：http://aqz.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://qcf.gzhubu.top

[R31] 局部变量
来源：http://zat.meibo888.top

f() { local x=1; echo "$x"; }
来源：http://eun.sysykeji.top

[R32] 参数个数校验
来源：http://pko.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://koa.0kj1m.cn

[R33] 捕获错误并提示行号
来源：http://tzc.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://adp.gzhubu.top

[R34] 退出时清理
来源：http://hpv.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://uow.daxiang520.top

[R35] 后台执行并等待
来源：http://olc.0kj1m.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://njg.svipenyu.cn

[R36] 并发执行多个任务
来源：http://dir.smart0.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dgx.smart0.xyz

[R37] 把输出赋给变量
来源：http://bgs.feifeiyinyue.top

files=$(ls -1)
来源：http://xzm.shzxlz.cn

[R38] 管道串联
来源：http://rdy.jqgufenzy.top

cat a.txt | grep -i error | wc -l
来源：http://xqm.ivvv.top

[R39] 重定向标准输出与错误
来源：http://ufc.sjlbkw.cn

cmd > out.log 2>&1
来源：http://ogm.xuanzx.com

[R40] 追加写日志
来源：http://mkp.wangshuangyany.cn

echo "log" >> out.log
来源：http://lmf.andypj.xyz

[R41] 丢弃输出
来源：http://zmg.jinghuilouyu.cn

cmd >/dev/null 2>&1
来源：http://geb.andypj.xyz

[R42] 输入重定向
来源：http://poi.pengpengdd.cyou

wc -l < a.txt
来源：http://zwf.jqgfzy.top

[R43] 按名字查找文件
来源：http://psj.bbcook.cn

find . -name "*.log" -type f
来源：http://fbk.kuanghao11.cn

[R44] 按修改时间查找
来源：http://erb.jiagoushi.top

find . -mtime -7 -type f
来源：http://qgy.jiagoushi.top

[R45] 批量删除
来源：http://kgz.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://cam.jyoumei.cn

[R46] 递归替换文件内容
来源：http://jxb.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zms.svipenyu.cn

[R47] sed 单行替换
来源：http://mod.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://nou.fengsongda.top

[R48] awk 取指定列
来源：http://wpx.fanxiaobao.xyz

awk '{print $1, $3}' a.txt
来源：http://lws.aizwys.cn

[R49] awk 带条件
来源：http://ora.cucudq.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://rnj.zhaomingkeji.xyz

[R50] awk 求和
来源：http://bwk.birdmap.top

awk '{s += $2} END {print s}' a.txt
来源：http://txl.hywenlv.cn

[R51] 排序去重取前几
来源：http://dff.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://dtm.zhaomingkeji.xyz

[R52] 统计行数
来源：http://vtv.sxryk.cn

wc -l a.txt
来源：http://mqs.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://szb.xuanzx.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://brc.tianlin.xyz

[R54] 比较两个文件
来源：http://tne.xuetiantiany.cn

diff a.txt b.txt
来源：http://rmo.guannengcc.top

[R55] 压缩与解压
来源：http://ply.chenzaomai.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://orb.hnxiangtu.top

[R56] 远程拷贝
来源：http://hoo.shuidangran.top

scp file user@host:/path/
来源：http://rqd.hfpthk.cn

[R57] 远程执行命令
来源：http://qko.jlsjyb.cn

ssh user@host 'uptime'
来源：http://rnc.sufxvd.cn

[R58] 下载文件
来源：http://tqh.yj20258888.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bem.haohaochexian.top

[R59] 发 POST JSON
来源：http://pop.yanxiufei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rcw.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://rig.yonumen.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://roj.vqdsnc.cn

[R61] 磁盘占用
来源：http://ijt.jqgufenzy.top

df -h;  du -sh *
来源：http://wfa.sjlbkw.cn

[R62] 找最占空间的文件
来源：http://cug.hnqzz.top

du -ah . | sort -rh | head -10
来源：http://uki.chenlongwang.top

[R63] 内存与进程
来源：http://gaa.gzhubu.top

free -h;  ps aux | grep nginx
来源：http://qbw.316326.xyz

[R64] 结束进程
来源：http://ewf.zhixingplan.top

kill -9 $(pgrep -f app.py)
来源：http://jxx.ydzc1.top

[R65] 查看端口占用
来源：http://qlr.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ocy.ctjpmb.com

[R66] 定时任务
来源：http://hjb.shuidangran.top

crontab -e;  crontab -l
来源：http://ppd.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://pmj.tanke756.top

openssl rand -hex 16
来源：http://ink.birdmap.top

[R68] 计算文件校验值
来源：http://uyi.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://acx.9152youxi.cn

[R69] 生成随机密码
来源：http://fzz.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://nwo.hnxiangtu.top

[R70] 时间戳与互转
来源：http://inq.andypj.xyz

date +%s;  date -d @1700000000
来源：http://qov.yonumen.top

[R71] 日期格式化
来源：http://uih.daxiang520.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://xiy.hammf.cn

[R72] 等待端口就绪
来源：http://npn.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://uqw.andypj.xyz

[R73] 分割大日志
来源：http://flc.fehbvm.com

split -l 1000 big.log part_
来源：http://rvn.jianghu66.top

[R74] 批量重命名
来源：http://xwh.sxryk.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mgf.quarkkingdee.top

[R75] 导出环境变量
来源：http://eaq.cashguo.top

export PATH="$HOME/bin:$PATH"
来源：http://vmp.fzhhl.top

[R76] 使用临时文件
来源：http://qan.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cbh.vqdsnc.cn

[R77] 读取用户输入
来源：http://zpd.pycfn.com

read -rp "请输入: " ans
来源：http://ffe.hnqzz.top

[R78] 交互式菜单
来源：http://qxb.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://svc.wangshuangyany.cn

[R79] 解析命令行选项
来源：http://gow.jiagoushi.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uta.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://kop.hammf.cn

time ./run.sh
来源：http://ykf.pycfn.com

================================================================================
来源：http://ngt.ivvv.top

S. C / C++ 专题
来源：http://prk.yvedp.cn

================================================================================
来源：http://nlv.yanxiufei.cn

[S01] C：Hello World
来源：http://mxh.snrcjt.cn

#include <stdio.h>
来源：http://wwh.zhixingplan.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oom.yvedp.cn

[S02] C：变量与格式化输出
来源：http://qag.yvedp.cn

int a = 10; printf("%d\n", a);
来源：http://gff.kuanghao11.cn

[S03] C：读入整数
来源：http://fal.havefunace.top

int x; scanf("%d", &x);
来源：http://knr.gogol.net.cn

[S04] C：字符串复制
来源：http://wng.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qnk.bjfxy.top

[S05] C：字符串长度
来源：http://cnu.fktsv.cn

strlen(s)
来源：http://ujo.smart0.xyz

[S06] C：字符串比较
来源：http://imb.uphjek.com

strcmp(a, b) == 0
来源：http://unh.fktsv.cn

[S07] C：数组遍历求和
来源：http://hgp.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hmq.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://utx.jinqigfzy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oej.xingfuxueyuan.xyz

[S09] C：结构体定义与初始化
来源：http://vuj.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yte.epnwcf.com

[S10] C：指针与解引用
来源：http://sip.ydjk.org.cn

int *p = &a;  *p = 5;
来源：http://qld.hammf.cn

[S11] C：逐行读文件
来源：http://jds.sweek.top

FILE *f = fopen("a.txt", "r");
来源：http://rio.hfpthk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dwd.xinyue.icu

fclose(f);
来源：http://eia.shuidangran.top

[S12] C：写文件
来源：http://zhc.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yir.yj202588.top

[S13] C：宏定义
来源：http://qrv.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pzu.aizwys.cn

[S14] C：枚举
来源：http://ywg.daria6918.cn

enum Color { RED, GREEN, BLUE };
来源：http://hxt.fzhhl.top

[S15] C：类型转换
来源：http://yqc.hongshengwenyu.top

(double) a / b
来源：http://wbm.guowangkeji.top

[S16] C：位操作置位
来源：http://fhf.yongpay.top

x |= (1 << 3);
来源：http://sra.c1oappe.top

[S17] C：安全拼接字符串
来源：http://ikv.c1oappe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pyn.birdmap.top

[S18] C：命令行参数
来源：http://jwh.ybcxt.top

int main(int argc, char **argv)
来源：http://wwx.hesvh.cn

[S19] C：快速排序
来源：http://abl.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://utt.svipenyu.cn

[S20] C：二分查找
来源：http://lvn.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uyc.yj20258.top

[S21] C：字符类别判断
来源：http://auq.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sql.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://xni.hywenlv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pqm.feifeiyinyue.top

[S23] C：随机数
来源：http://pqb.daria6918.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xsi.wangshuangyany.cn

[S24] C：获取本地时间
来源：http://tch.jinqigufen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qmd.hnqzz.top

[S25] C：内存拷贝
来源：http://czc.fzhhl.top

memcpy(dst, src, n);
来源：http://kya.hfpthk.cn

[S26] C：内存清零
来源：http://uxq.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://qhe.fzhhl.top

[S27] C：定义常量
来源：http://qzx.zhoulong.xyz

const double PI = 3.14159;
来源：http://obp.yuxming.cn

[S28] C：静态变量
来源：http://bhc.ivvv.top

static int counter = 0;
来源：http://lfz.jlsjyb.cn

[S29] C：变参函数
来源：http://hsm.gzhubu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xjc.shuidangran.top

[S30] C：头文件保护
来源：http://gif.chenjidiqi.icu

#ifndef X_H
来源：http://ajq.uphjek.com

#define X_H
来源：http://ktu.cqqwz.cn

#endif
来源：http://ujx.wangshuangyany.cn

[S31] C++：Hello World
来源：http://eph.yueranfly.top

#include <iostream>
来源：http://crh.zdbjq.cn

int main() { std::cout << "Hello\n"; }
来源：http://tpw.hfpthk.cn

[S32] C++：字符串
来源：http://zea.redwolf501.top

std::string s = "hi";  s += "!";
来源：http://udq.yvedp.cn

[S33] C++：vector 增删
来源：http://bqh.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vit.ctjpmb.com

[S34] C++：遍历 vector
来源：http://vwl.xziqi.cn

for (auto &x : v) { std::cout << x; }
来源：http://kih.ivvv.top

[S35] C++：map
来源：http://vhb.0kj1m.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kid.bjfxy.top

[S36] C++：unordered_map
来源：http://pjt.hnxiangtu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://egi.hesvh.cn

[S37] C++：set
来源：http://eyv.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tkl.hesvh.cn

[S38] C++：排序
来源：http://frl.yuxming.cn

std::sort(v.begin(), v.end());
来源：http://ovk.yj20258888.top

[S39] C++：自定义比较器排序
来源：http://eii.xylfe.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vuq.yj20258.top

[S40] C++：查找元素
来源：http://dyp.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iie.uphjek.com

[S41] C++：类与构造函数
来源：http://yem.c1oappe.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://czh.cheryme.top

[S42] C++：继承与虚函数
来源：http://ejn.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://hoj.shuidangran.top


<!-- 参考信息 -->