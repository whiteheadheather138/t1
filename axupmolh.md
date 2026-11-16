代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qnc.ctjpmb.com

[Q58] 累计求和
来源：http://qty.xinyue.icu

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jkm.pycfn.com

[Q59] 分组内累计
来源：http://luz.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mhs.tianlin.xyz

[Q60] 取上一行 / 下一行
来源：http://oss.jinyuanbaomall.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hfr.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://bjj.shanyushiyangtech.top

[Q61] 移动平均
来源：http://pxj.meibo888.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dzn.zhaomingkeji.xyz

[Q62] 分组占比
来源：http://xev.zycfv.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://izq.yj202588.top

[Q63] 开启事务
来源：http://prs.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://okm.chenzaomai.com

[Q64] 提交事务
来源：http://afy.jinyuanbaomall.cn

COMMIT;
来源：http://mal.birdmap.top

[Q65] 回滚事务
来源：http://sqj.tanke756.top

ROLLBACK;
来源：http://cwj.bjfxy.top

[Q66] 行锁查询
来源：http://byy.aizwys.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ibt.xuanzx.com

[Q67] 设置隔离级别
来源：http://fil.yangfankeji.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xcx.bbcook.cn

[Q68] 保存点
来源：http://gfe.ivvv.top

SAVEPOINT sp1;
来源：http://cow.uphjek.com

ROLLBACK TO sp1;
来源：http://kxf.bjfxy.top

[Q69] 查看执行计划
来源：http://upv.andypj.xyz

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kih.bjfxy.top

[Q70] 更新统计信息
来源：http://qnb.chenlongwang.top

ANALYZE TABLE users;
来源：http://pmx.zdqjudy.top

[Q71] 查看建表语句
来源：http://rfn.yongpay.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://phk.hnqzz.top

[Q72] 查看索引
来源：http://uae.daria6918.cn

SHOW INDEX FROM users;
来源：http://ogf.yuanzhike.top

[Q73] 查看表状态
来源：http://ayk.yonumen.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pfk.9152youxi.cn

[Q74] 强制使用索引
来源：http://rba.pycfn.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mew.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://ani.redwolf501.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hkn.sysykeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mjz.pycfn.com

[Q76] 按天统计
来源：http://jil.jinqigfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://obu.yj20258.top

[Q77] 时间加减
来源：http://nsg.bbcook.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gjh.nanxuanxn.top

[Q78] 当前时间
来源：http://jyb.fktsv.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zcu.sufxvd.cn

[Q79] 字符串拼接
来源：http://tor.redwolf501.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://boz.bbcook.cn

[Q80] 字符串截取
来源：http://eiy.hywenlv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yef.hnqzz.top

[Q81] 字符串替换
来源：http://mbo.ydzc1.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dcr.gogol.net.cn

[Q82] 字符长度与字节长度
来源：http://fxt.yangfankeji.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pzk.wangshuangyany.cn

[Q83] 大小写转换
来源：http://qua.sufxvd.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://oud.xinyue.icu

[Q84] 去除首尾空格
来源：http://czd.sweek.top

SELECT TRIM(name) FROM users;
来源：http://taj.ybcxt.top

[Q85] 数值取整
来源：http://yxq.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jmu.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://kpf.shanyushiyangkeji.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yxe.jinqigufen.top

[Q87] JSON 字段做条件
来源：http://cth.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://lre.smart0.xyz

[Q88] 行转列（条件聚合）
来源：http://fxm.0kj1m.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vof.andypj.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://vgx.zdbjq.cn

[Q89] 判断表是否存在
来源：http://ins.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mod.sjlbkw.cn

[Q90] 生成序号列
来源：http://qid.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://crz.shanyushiyangtech.top

================================================================================
来源：http://dqx.xziqi.cn

R. Bash 专题
来源：http://dwn.vqdsnc.cn

================================================================================
来源：http://wam.vqdsnc.cn

[R01] shebang 与严格模式
来源：http://osr.ydjk.org.cn

#!/usr/bin/env bash
来源：http://miw.shanyushiyangkeji.top

set -euo pipefail
来源：http://txn.yfazqb.com

[R02] 变量赋值与使用
来源：http://hlu.nanxuanxn.top

name="Tom"; echo "$name"
来源：http://gro.dianchejie.cn

[R03] 只读变量
来源：http://qgo.cdnleiting.top

readonly PI=3.14
来源：http://xto.yongpay.top

[R04] 位置参数
来源：http://ide.jqgufenzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dyk.gotoacloud.top

[R05] 参数默认值
来源：http://iar.sjlbkw.cn

name="${1:-default}"
来源：http://jup.svipenyu.cn

[R06] 判断命令是否存在
来源：http://vcy.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cle.0kj1m.cn

[R07] if 判断文件
来源：http://ure.cashguo.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ekp.zhoulong.xyz

[R08] 数值比较
来源：http://fzn.shuidangran.top

if (( a > b )); then echo "a 更大"; fi
来源：http://lve.ybcxt.top

[R09] 字符串比较
来源：http://ooe.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://swu.mhx1999.top

[R10] 正则匹配
来源：http://bqi.yj20258888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ura.yonumen.top

[R11] case 多分支
来源：http://ypu.gaohongyu789.top

case "$1" in
来源：http://gsj.havefunace.top

start) echo "启动" ;;
来源：http://cxq.hcnkem.com

stop)  echo "停止" ;;
来源：http://akq.sweek.top

*)     echo "未知命令" ;;
来源：http://kjd.uphjek.com

esac
来源：http://pju.gogol.net.cn

[R12] for 遍历文件
来源：http://lli.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://pgz.0kj1m.cn

[R13] for 计数循环
来源：http://suc.aizwys.cn

for i in {1..10}; do echo "$i"; done
来源：http://zbk.yueranfly.top

[R14] C 风格 for
来源：http://bxw.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://eok.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://yzr.zhaomingkeji.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sgy.cqqwz.cn

[R16] until 等待条件
来源：http://bdd.smart0.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qiu.jqgfzy.top

[R17] 数组定义与取值
来源：http://jwn.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://oqk.jinghuilouyu.cn

[R18] 遍历数组
来源：http://gig.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uuc.yvedp.cn

[R19] 数组长度
来源：http://klv.yonumen.top

echo "${#arr[@]}"
来源：http://zxo.fanxiaobao.xyz

[R20] 关联数组（字典）
来源：http://tif.zhaomingkeji.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ohl.pycfn.com

[R21] 字符串长度
来源：http://pxa.yj20258888.top

echo "${#s}"
来源：http://rhs.zhijiandao.cn

[R22] 截取子串
来源：http://dnf.ivvv.top

echo "${s:0:5}"
来源：http://wfm.ybcxt.top

[R23] 字符串替换
来源：http://mvr.cheryme.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gxn.tarul.cn

[R24] 大小写转换
来源：http://wta.fktsv.cn

echo "${s^^}"; echo "${s,,}"
来源：http://reo.jinghuilouyu.cn

[R25] 去后缀 / 去前缀
来源：http://rxe.zhaomingkeji.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://ftu.mhx1999.top

[R26] 命令替换
来源：http://ykk.zhaomingkeji.xyz

now=$(date +%F); echo "$now"
来源：http://ckc.zdqjudy.top

[R27] 算术展开
来源：http://jup.guannengcc.top

echo $((1 + 2 * 3))
来源：http://bxy.yvedp.cn

[R28] 浮点运算
来源：http://cvt.meibo888.top

echo "scale=2; 10/3" | bc
来源：http://nkc.sufxvd.cn

[R29] 定义函数
来源：http://tem.gaohongyu789.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dmp.zdbjq.cn

[R30] 函数返回状态码
来源：http://wnz.yongpay.top

f() { return 0; }; f || echo "失败了"
来源：http://duu.cheryme.top

[R31] 局部变量
来源：http://tyu.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://qzg.feifeiyinyue.top

[R32] 参数个数校验
来源：http://mwt.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mzc.tanke756.top

[R33] 捕获错误并提示行号
来源：http://byf.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nnh.cqqwz.cn

[R34] 退出时清理
来源：http://qrh.zycfv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://wfj.quarkkingdee.top

[R35] 后台执行并等待
来源：http://vlw.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rnb.daria6918.cn

[R36] 并发执行多个任务
来源：http://fxt.birdmap.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dhh.tarul.cn

[R37] 把输出赋给变量
来源：http://dil.ppjwa.cn

files=$(ls -1)
来源：http://mjv.cucudq.cn

[R38] 管道串联
来源：http://qin.fengsongda.top

cat a.txt | grep -i error | wc -l
来源：http://bzf.meibo888.top

[R39] 重定向标准输出与错误
来源：http://aoj.daxiang520.top

cmd > out.log 2>&1
来源：http://gyt.mhx1999.top

[R40] 追加写日志
来源：http://xew.guowangkeji.top

echo "log" >> out.log
来源：http://wzl.yj202588.top

[R41] 丢弃输出
来源：http://vgc.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://ojd.shanyushiyangtech.top

[R42] 输入重定向
来源：http://nvk.ywan-chungtsiang.top

wc -l < a.txt
来源：http://cti.yangfankeji.com

[R43] 按名字查找文件
来源：http://ppo.yuanzhike.top

find . -name "*.log" -type f
来源：http://qos.fzhhl.top

[R44] 按修改时间查找
来源：http://rbo.chenlongwang.top

find . -mtime -7 -type f
来源：http://nzb.tianlin.xyz

[R45] 批量删除
来源：http://yhr.hesvh.cn

find . -name "*.tmp" -delete
来源：http://gwp.zycfv.cn

[R46] 递归替换文件内容
来源：http://sau.yj202588.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://woc.nanxuanxn.top

[R47] sed 单行替换
来源：http://tip.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://jih.hnqzz.top

[R48] awk 取指定列
来源：http://xqz.xuanzx.com

awk '{print $1, $3}' a.txt
来源：http://bsa.hfpthk.cn

[R49] awk 带条件
来源：http://iju.zhongyouzk.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nlp.cashguo.top

[R50] awk 求和
来源：http://jbs.cashguo.top

awk '{s += $2} END {print s}' a.txt
来源：http://eek.shuidangran.top

[R51] 排序去重取前几
来源：http://avi.jqgufenzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sgm.cheryme.top

[R52] 统计行数
来源：http://cby.ehwqpu.com

wc -l a.txt
来源：http://dtq.jqgfzy.top

[R53] 查看文件头与实时尾
来源：http://yhh.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbk.birdmap.top

[R54] 比较两个文件
来源：http://qdw.0kj1m.cn

diff a.txt b.txt
来源：http://vpa.yvedp.cn

[R55] 压缩与解压
来源：http://qge.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xao.kuanghao11.cn

[R56] 远程拷贝
来源：http://kgt.bjfxy.top

scp file user@host:/path/
来源：http://mwu.wangshuangyany.cn

[R57] 远程执行命令
来源：http://xia.c1oappe.top

ssh user@host 'uptime'
来源：http://ktd.zdbjq.cn

[R58] 下载文件
来源：http://gge.ydzc1.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hcs.aizwys.cn

[R59] 发 POST JSON
来源：http://lps.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rha.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://lmh.guowangkeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://exi.hammf.cn

[R61] 磁盘占用
来源：http://dln.yfazqb.com

df -h;  du -sh *
来源：http://hwq.xuetiantiany.cn

[R62] 找最占空间的文件
来源：http://frg.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://mad.snrcjt.cn

[R63] 内存与进程
来源：http://crs.chenzaomai.com

free -h;  ps aux | grep nginx
来源：http://jnv.iojbl.cn

[R64] 结束进程
来源：http://smo.hfpthk.cn

kill -9 $(pgrep -f app.py)
来源：http://heu.tarul.cn

[R65] 查看端口占用
来源：http://nzn.xingfuxueyuan.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uqf.cdnleiting.top

[R66] 定时任务
来源：http://ove.mhx1999.top

crontab -e;  crontab -l
来源：http://wpd.wangdashe.top

[R67] 生成随机十六进制串
来源：http://bme.cucudq.cn

openssl rand -hex 16
来源：http://wqi.dashuyun.cn

[R68] 计算文件校验值
来源：http://iuq.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://krl.pycfn.com

[R69] 生成随机密码
来源：http://qub.zhixingplan.top

head -c 16 /dev/urandom | base64
来源：http://npu.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://crl.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://bpi.wangshuangyany.cn

[R71] 日期格式化
来源：http://rqt.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cai.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://yzc.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bba.yanxiufei.cn

[R73] 分割大日志
来源：http://zuw.zhengqikj.top

split -l 1000 big.log part_
来源：http://yew.ydjk.org.cn

[R74] 批量重命名
来源：http://hzz.0kj1m.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ivk.sysykeji.top

[R75] 导出环境变量
来源：http://xem.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://ael.fzhhl.top

[R76] 使用临时文件
来源：http://umy.yueranfly.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tjm.xuetiantiany.cn

[R77] 读取用户输入
来源：http://hnv.yueranfly.top

read -rp "请输入: " ans
来源：http://njy.fengsongda.top

[R78] 交互式菜单
来源：http://rut.zhengqikj.top

select opt in a b c; do echo "$opt"; break; done
来源：http://klu.ppjwa.cn

[R79] 解析命令行选项
来源：http://oou.redwolf501.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qry.ivvv.top

[R80] 查看脚本执行耗时
来源：http://ykt.havefunace.top

time ./run.sh
来源：http://dsi.jqgufenzy.top

================================================================================
来源：http://juz.316326.xyz

S. C / C++ 专题
来源：http://arg.xziqi.cn

================================================================================
来源：http://lfh.zhongyouzk.top

[S01] C：Hello World
来源：http://hrk.xinyue.icu

#include <stdio.h>
来源：http://wur.9152youxi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tfa.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://sbv.fanxiaobao.xyz

int a = 10; printf("%d\n", a);
来源：http://wjv.zdqjudy.top

[S03] C：读入整数
来源：http://dij.zycfv.cn

int x; scanf("%d", &x);
来源：http://vna.wangshuangyany.cn

[S04] C：字符串复制
来源：http://apg.cucudq.cn

char dst[32]; strcpy(dst, "hi");
来源：http://pqt.iojbl.cn

[S05] C：字符串长度
来源：http://dhq.316326.xyz

strlen(s)
来源：http://njd.chenzaomai.com

[S06] C：字符串比较
来源：http://wih.havefunace.top

strcmp(a, b) == 0
来源：http://iwp.ehwqpu.com

[S07] C：数组遍历求和
来源：http://xvz.sufxvd.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tmj.guowangkeji.top

[S08] C：动态内存分配与释放
来源：http://rkp.dianchejie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rpv.dashuyun.cn

[S09] C：结构体定义与初始化
来源：http://jlb.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://exf.havefunace.top

[S10] C：指针与解引用
来源：http://qqo.xziqi.cn

int *p = &a;  *p = 5;
来源：http://lao.yuxming.cn

[S11] C：逐行读文件
来源：http://fec.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://dwm.redwolf501.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://vdh.xylfe.cn

fclose(f);
来源：http://hsz.aibaodan.cn

[S12] C：写文件
来源：http://jwx.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jrc.hcnkem.com

[S13] C：宏定义
来源：http://tkh.shuidangran.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xai.chenlongwang.top

[S14] C：枚举
来源：http://aki.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://hiv.gogol.net.cn

[S15] C：类型转换
来源：http://vcc.xuanzx.com

(double) a / b
来源：http://cvo.ivvv.top

[S16] C：位操作置位
来源：http://sax.yangfankeji.com

x |= (1 << 3);
来源：http://xni.cashguo.top

[S17] C：安全拼接字符串
来源：http://fyr.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jjh.gogol.net.cn

[S18] C：命令行参数
来源：http://bog.fzhhl.top

int main(int argc, char **argv)
来源：http://vvh.xingfuxueyuan.xyz

[S19] C：快速排序
来源：http://mip.jqgufenzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://mtm.jinyuanbaomall.cn

[S20] C：二分查找
来源：http://tjq.yangfankeji.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lpl.xingfuxueyuan.xyz

[S21] C：字符类别判断
来源：http://jyj.jianghu66.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zou.ydjk.org.cn

[S22] C：字符串转数字
来源：http://nmv.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://efl.guowangkeji.top

[S23] C：随机数
来源：http://tkr.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://epl.fanxiaobao.xyz

[S24] C：获取本地时间
来源：http://zvx.jinqigfzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://haw.gotoacloud.top

[S25] C：内存拷贝
来源：http://qte.cucudq.cn

memcpy(dst, src, n);
来源：http://ckl.epnwcf.com

[S26] C：内存清零
来源：http://kwz.shzxlz.cn

memset(a, 0, sizeof a);
来源：http://jhv.cashguo.top

[S27] C：定义常量
来源：http://opr.iojbl.cn

const double PI = 3.14159;
来源：http://qcf.52xcode.cn

[S28] C：静态变量
来源：http://lea.epnwcf.com


<!-- 参考信息 -->