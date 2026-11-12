代发 wailian999

[Q65] 回滚事务
来源：http://ywk.yuxming.cn

ROLLBACK;
来源：http://ggz.sysykeji.top

[Q66] 行锁查询
来源：http://qpa.svipenyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qee.52xcode.cn

[Q67] 设置隔离级别
来源：http://eff.gogol.net.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://efm.yj20258888.top

[Q68] 保存点
来源：http://oka.zhengqikj.top

SAVEPOINT sp1;
来源：http://zqy.hnqzz.top

ROLLBACK TO sp1;
来源：http://fce.sxryk.cn

[Q69] 查看执行计划
来源：http://acr.9152youxi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://lgx.iojbl.cn

[Q70] 更新统计信息
来源：http://lmd.shanyushiyangkeji.top

ANALYZE TABLE users;
来源：http://eah.52xcode.cn

[Q71] 查看建表语句
来源：http://vmn.sjlbkw.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iiu.hnqzz.top

[Q72] 查看索引
来源：http://zzw.ydzc1.top

SHOW INDEX FROM users;
来源：http://qsa.aibaodan.cn

[Q73] 查看表状态
来源：http://tks.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://rcz.redwolf501.top

[Q74] 强制使用索引
来源：http://tbw.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sor.hnqzz.top

[Q75] 日期格式化
来源：http://ktf.sweek.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://jee.zhixingplan.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lhw.pengpengdd.cyou

[Q76] 按天统计
来源：http://yie.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://pcu.xinyue.icu

[Q77] 时间加减
来源：http://wan.andypj.xyz

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://smk.jiagoushi.top

[Q78] 当前时间
来源：http://dre.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jbq.0kj1m.cn

[Q79] 字符串拼接
来源：http://ant.shangyingyoupin.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pxs.epnwcf.com

[Q80] 字符串截取
来源：http://yyp.yangfankeji.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lgv.jinyuanbaomall.cn

[Q81] 字符串替换
来源：http://agx.jinyuanbaomall.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://bqn.feifeiyinyue.top

[Q82] 字符长度与字节长度
来源：http://trj.zhijiandao.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oiw.vqdsnc.cn

[Q83] 大小写转换
来源：http://vqq.fzhhl.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qcd.0kj1m.cn

[Q84] 去除首尾空格
来源：http://wbc.gogol.net.cn

SELECT TRIM(name) FROM users;
来源：http://skj.meibo888.top

[Q85] 数值取整
来源：http://qcs.shanyushiyangtech.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xqf.hesvh.cn

[Q86] 读取 JSON 字段
来源：http://lzz.shangyingyoupin.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://att.ivvv.top

[Q87] JSON 字段做条件
来源：http://kox.vqdsnc.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://bkv.ivvv.top

[Q88] 行转列（条件聚合）
来源：http://alg.chenzaomai.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ukt.ctjpmb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://uhp.shuidangran.top

[Q89] 判断表是否存在
来源：http://xdh.yongpay.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hgl.wangdashe.top

[Q90] 生成序号列
来源：http://sku.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tjq.guowangkeji.top

================================================================================
来源：http://imt.bbcook.cn

R. Bash 专题
来源：http://icl.daria6918.cn

================================================================================
来源：http://lnk.meibo888.top

[R01] shebang 与严格模式
来源：http://cra.yj20258.top

#!/usr/bin/env bash
来源：http://bgk.svipenyu.cn

set -euo pipefail
来源：http://uyr.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://acd.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://ptd.316326.xyz

[R03] 只读变量
来源：http://ewl.yonumen.top

readonly PI=3.14
来源：http://rfb.cqqwz.cn

[R04] 位置参数
来源：http://scv.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://roq.jlsjyb.cn

[R05] 参数默认值
来源：http://hwf.sweek.top

name="${1:-default}"
来源：http://qxp.aizwys.cn

[R06] 判断命令是否存在
来源：http://xye.chenjidiqi.icu

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iug.xinyue.icu

[R07] if 判断文件
来源：http://udo.bjfxy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wfb.jlsjyb.cn

[R08] 数值比较
来源：http://cuz.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jyk.xuetiantiany.cn

[R09] 字符串比较
来源：http://aif.cqqwz.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://axz.pycfn.com

[R10] 正则匹配
来源：http://lkr.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qea.9152youxi.cn

[R11] case 多分支
来源：http://szi.shuidangran.top

case "$1" in
来源：http://gex.52xcode.cn

start) echo "启动" ;;
来源：http://sna.ehwqpu.com

stop)  echo "停止" ;;
来源：http://qnn.tanke756.top

*)     echo "未知命令" ;;
来源：http://iop.zhijiandao.cn

esac
来源：http://fbu.epnwcf.com

[R12] for 遍历文件
来源：http://dqw.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://gxb.hnxiangtu.top

[R13] for 计数循环
来源：http://qrs.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://zzn.cqqwz.cn

[R14] C 风格 for
来源：http://lby.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://spl.zhixingplan.top

[R15] while 逐行读文件
来源：http://iys.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jap.nwbrower.top

[R16] until 等待条件
来源：http://jjr.cdnleiting.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rdc.gogol.net.cn

[R17] 数组定义与取值
来源：http://fyk.fanxiaobao.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://mbf.sysykeji.top

[R18] 遍历数组
来源：http://kuc.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wfa.zdqjudy.top

[R19] 数组长度
来源：http://qiq.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://fuz.hammf.cn

[R20] 关联数组（字典）
来源：http://szj.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://adl.aibaodan.cn

[R21] 字符串长度
来源：http://ara.ydjk.org.cn

echo "${#s}"
来源：http://czj.cashguo.top

[R22] 截取子串
来源：http://kls.chenzaomai.com

echo "${s:0:5}"
来源：http://maq.bbcook.cn

[R23] 字符串替换
来源：http://tji.xuetiantiany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fgn.316326.xyz

[R24] 大小写转换
来源：http://xfh.birdmap.top

echo "${s^^}"; echo "${s,,}"
来源：http://rzf.zhaomingkeji.xyz

[R25] 去后缀 / 去前缀
来源：http://pwh.gogol.net.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://kwo.zhoulong.xyz

[R26] 命令替换
来源：http://tpv.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://vvn.gzhubu.top

[R27] 算术展开
来源：http://gmi.xingfuxueyuan.xyz

echo $((1 + 2 * 3))
来源：http://edy.guannengcc.top

[R28] 浮点运算
来源：http://xvc.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://vgj.zhaomingkeji.xyz

[R29] 定义函数
来源：http://nkg.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kmv.smart0.xyz

[R30] 函数返回状态码
来源：http://cvm.zhoulong.xyz

f() { return 0; }; f || echo "失败了"
来源：http://slm.haohaochexian.top

[R31] 局部变量
来源：http://ykx.ybcxt.top

f() { local x=1; echo "$x"; }
来源：http://rkd.svipenyu.cn

[R32] 参数个数校验
来源：http://vqs.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://muj.cheryme.top

[R33] 捕获错误并提示行号
来源：http://enj.zhongyouzk.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wir.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://bcy.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://egw.haohaochexian.top

[R35] 后台执行并等待
来源：http://tjv.zdbjq.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://qzi.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://xdi.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xho.ybcxt.top

[R37] 把输出赋给变量
来源：http://hez.yvedp.cn

files=$(ls -1)
来源：http://zoe.smart0.xyz

[R38] 管道串联
来源：http://tmz.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://dfa.yuxming.cn

[R39] 重定向标准输出与错误
来源：http://mhk.fzhhl.top

cmd > out.log 2>&1
来源：http://jre.iojbl.cn

[R40] 追加写日志
来源：http://jcc.cdnleiting.top

echo "log" >> out.log
来源：http://coj.havefunace.top

[R41] 丢弃输出
来源：http://rec.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://cco.aibaodan.cn

[R42] 输入重定向
来源：http://les.jlsjyb.cn

wc -l < a.txt
来源：http://ijl.nanxuanxn.top

[R43] 按名字查找文件
来源：http://aop.fengsongda.top

find . -name "*.log" -type f
来源：http://eve.zhongyouzk.top

[R44] 按修改时间查找
来源：http://kgm.yanxiufei.cn

find . -mtime -7 -type f
来源：http://drl.zhiwuduotai.top

[R45] 批量删除
来源：http://zdg.andypj.xyz

find . -name "*.tmp" -delete
来源：http://fne.zhongyouzk.top

[R46] 递归替换文件内容
来源：http://eqv.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://psz.sjlbkw.cn

[R47] sed 单行替换
来源：http://hah.ehwqpu.com

sed -i 's/foo/bar/g' a.txt
来源：http://ujo.yj20258888.top

[R48] awk 取指定列
来源：http://fam.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://obb.ydzc1.top

[R49] awk 带条件
来源：http://yqj.xuanzx.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://epj.shanyushiyangkeji.top

[R50] awk 求和
来源：http://eip.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://kco.cucudq.cn

[R51] 排序去重取前几
来源：http://veh.yj20258.top

sort a.txt | uniq -c | sort -rn | head
来源：http://hsr.zhaomingkeji.xyz

[R52] 统计行数
来源：http://blk.ybcxt.top

wc -l a.txt
来源：http://eow.dianchejie.cn

[R53] 查看文件头与实时尾
来源：http://fuo.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nbl.guowangkeji.top

[R54] 比较两个文件
来源：http://tum.nanxinkj.top

diff a.txt b.txt
来源：http://vvu.chenjidiqi.icu

[R55] 压缩与解压
来源：http://nru.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uxg.ybcxt.top

[R56] 远程拷贝
来源：http://bja.aizwys.cn

scp file user@host:/path/
来源：http://skv.wangdashe.top

[R57] 远程执行命令
来源：http://azt.guannengcc.top

ssh user@host 'uptime'
来源：http://grl.cqqwz.cn

[R58] 下载文件
来源：http://arc.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://veh.mhx1999.top

[R59] 发 POST JSON
来源：http://hqx.hfpthk.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kpy.cqqwz.cn

[R60] 只看 HTTP 状态码
来源：http://dbp.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xrg.yuanzhike.top

[R61] 磁盘占用
来源：http://wfb.yj20258.top

df -h;  du -sh *
来源：http://brp.yuxming.cn

[R62] 找最占空间的文件
来源：http://kkv.sweek.top

du -ah . | sort -rh | head -10
来源：http://jqj.yongpay.top

[R63] 内存与进程
来源：http://cpc.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://wof.feifeiyinyue.top

[R64] 结束进程
来源：http://rub.jlsjyb.cn

kill -9 $(pgrep -f app.py)
来源：http://evn.nwbrower.top

[R65] 查看端口占用
来源：http://jsn.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://axe.316326.xyz

[R66] 定时任务
来源：http://jhd.wangdashe.top

crontab -e;  crontab -l
来源：http://vwe.fzhhl.top

[R67] 生成随机十六进制串
来源：http://uyv.yuxming.cn

openssl rand -hex 16
来源：http://mdu.ywan-chungtsiang.top

[R68] 计算文件校验值
来源：http://wfr.zhengqikj.top

sha256sum a.txt;  md5sum a.txt
来源：http://vnw.tianlin.xyz

[R69] 生成随机密码
来源：http://jgw.shanyushiyangkeji.top

head -c 16 /dev/urandom | base64
来源：http://mvq.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://vsa.bbcook.cn

date +%s;  date -d @1700000000
来源：http://clj.fktsv.cn

[R71] 日期格式化
来源：http://foq.zhiwuduotai.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kqo.kuanghao11.cn

[R72] 等待端口就绪
来源：http://tbl.wangdashe.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xdx.sysykeji.top

[R73] 分割大日志
来源：http://ivy.jianghu66.top

split -l 1000 big.log part_
来源：http://oea.c1oappe.top

[R74] 批量重命名
来源：http://fll.shanyushiyangtech.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qva.bjfxy.top

[R75] 导出环境变量
来源：http://oui.jyoumei.cn

export PATH="$HOME/bin:$PATH"
来源：http://xar.jianghu66.top

[R76] 使用临时文件
来源：http://qlx.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jve.chenlongwang.top

[R77] 读取用户输入
来源：http://vym.xingfuxueyuan.xyz

read -rp "请输入: " ans
来源：http://yrq.yj20258.top

[R78] 交互式菜单
来源：http://uxz.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ggp.pycfn.com

[R79] 解析命令行选项
来源：http://jyu.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://cok.shanyushiyangkeji.top

[R80] 查看脚本执行耗时
来源：http://wqd.snrcjt.cn

time ./run.sh
来源：http://rcp.jinyuanbaomall.cn

================================================================================
来源：http://rds.zdbjq.cn

S. C / C++ 专题
来源：http://brn.fanxiaobao.xyz

================================================================================
来源：http://amy.vqdsnc.cn

[S01] C：Hello World
来源：http://jhr.shzxlz.cn

#include <stdio.h>
来源：http://qxk.xuanzx.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://vdv.aibaodan.cn

[S02] C：变量与格式化输出
来源：http://hiz.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://ekz.xuanzx.com

[S03] C：读入整数
来源：http://ngl.redwolf501.top

int x; scanf("%d", &x);
来源：http://clr.cqqwz.cn

[S04] C：字符串复制
来源：http://rgw.hnxiangtu.top

char dst[32]; strcpy(dst, "hi");
来源：http://qaf.kuanghao11.cn

[S05] C：字符串长度
来源：http://yxq.52xcode.cn

strlen(s)
来源：http://fyc.andypj.xyz

[S06] C：字符串比较
来源：http://txk.shanyushiyangtech.top

strcmp(a, b) == 0
来源：http://vgr.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://fpv.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hhz.yj20258.top

[S08] C：动态内存分配与释放
来源：http://hor.tianlin.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://htc.feifeiyinyue.top

[S09] C：结构体定义与初始化
来源：http://nex.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dlm.guowangkeji.top

[S10] C：指针与解引用
来源：http://xut.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://fmh.cheryme.top

[S11] C：逐行读文件
来源：http://cjs.jlsjyb.cn

FILE *f = fopen("a.txt", "r");
来源：http://cem.9152youxi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://iun.bbcook.cn

fclose(f);
来源：http://zaq.aizwys.cn

[S12] C：写文件
来源：http://lhi.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ghx.wangdashe.top

[S13] C：宏定义
来源：http://qdl.yfazqb.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ozw.zhiwuduotai.top

[S14] C：枚举
来源：http://xyw.xinyue.icu

enum Color { RED, GREEN, BLUE };
来源：http://jmz.xingfuxueyuan.xyz

[S15] C：类型转换
来源：http://kej.fktsv.cn

(double) a / b
来源：http://big.sufxvd.cn

[S16] C：位操作置位
来源：http://lsc.xingfuxueyuan.xyz

x |= (1 << 3);
来源：http://pxe.yj20258888.top

[S17] C：安全拼接字符串
来源：http://jrc.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yuh.bbcook.cn

[S18] C：命令行参数
来源：http://ckk.cqqwz.cn

int main(int argc, char **argv)
来源：http://mly.hysaishi.cn

[S19] C：快速排序
来源：http://uve.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://xyu.kuanghao11.cn

[S20] C：二分查找
来源：http://qrt.nwbrower.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gcz.jqgufenzy.top

[S21] C：字符类别判断
来源：http://cei.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://slq.snrcjt.cn

[S22] C：字符串转数字
来源：http://wlc.zycfv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ujx.svipenyu.cn

[S23] C：随机数
来源：http://eew.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vxf.c1oappe.top

[S24] C：获取本地时间
来源：http://npt.hfpthk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ycr.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://tca.yueranfly.top

memcpy(dst, src, n);
来源：http://bms.yfazqb.com

[S26] C：内存清零
来源：http://pwo.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://tay.ybcxt.top

[S27] C：定义常量
来源：http://kwg.hnxiangtu.top

const double PI = 3.14159;
来源：http://gah.smart0.xyz

[S28] C：静态变量
来源：http://mtw.tarul.cn

static int counter = 0;
来源：http://bzy.kuanghao11.cn

[S29] C：变参函数
来源：http://nzx.guowangkeji.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iod.9152youxi.cn

[S30] C：头文件保护
来源：http://wcf.yuanzhike.top

#ifndef X_H
来源：http://wlr.zdbjq.cn

#define X_H
来源：http://bcv.cucudq.cn

#endif
来源：http://yck.yongpay.top

[S31] C++：Hello World
来源：http://auh.jqgufenzy.top

#include <iostream>
来源：http://hji.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://tuu.9152youxi.cn

[S32] C++：字符串
来源：http://xqi.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://ppd.zdqjudy.top

[S33] C++：vector 增删
来源：http://xfk.zhixingplan.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wmb.feifeiyinyue.top

[S34] C++：遍历 vector
来源：http://lcu.yangfankeji.com

for (auto &x : v) { std::cout << x; }
来源：http://flt.ydzc1.top


<!-- 参考信息 -->